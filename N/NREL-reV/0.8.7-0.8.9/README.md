# Comparing `tmp/NREL-reV-0.8.7.tar.gz` & `tmp/NREL-reV-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-reV-0.8.7.tar", last modified: Thu Mar  7 18:57:19 2024, max compression
+gzip compressed data, was "NREL-reV-0.8.9.tar", last modified: Thu May 30 19:50:04 2024, max compression
```

## Comparing `NREL-reV-0.8.7.tar` & `NREL-reV-0.8.9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.805008 NREL-reV-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.789008 NREL-reV-0.8.7/NREL_reV.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-07 18:57:19.000000 NREL-reV-0.8.7/NREL_reV.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-07 18:57:19.000000 NREL-reV-0.8.7/NREL_reV.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 18:57:19.000000 NREL-reV-0.8.7/NREL_reV.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-07 18:57:19.000000 NREL-reV-0.8.7/NREL_reV.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 18:57:19.000000 NREL-reV-0.8.7/NREL_reV.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-07 18:57:19.000000 NREL-reV-0.8.7/NREL_reV.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-07 18:57:19.000000 NREL-reV-0.8.7/NREL_reV.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-03-07 18:57:19.805008 NREL-reV-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.793008 NREL-reV-0.8.7/reV/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.793008 NREL-reV-0.8.7/reV/SAM/
--rw-r--r--   0 runner    (1001) docker     (127)    30422 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/SAM/SAM.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/SAM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/SAM/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/SAM/econ.py
--rw-r--r--   0 runner    (1001) docker     (127)    86060 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/SAM/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/SAM/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/SAM/windbos.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.793008 NREL-reV-0.8.7/reV/bespoke/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/bespoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   101746 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/bespoke/bespoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/bespoke/cli_bespoke.py
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/bespoke/gradient_free.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/bespoke/pack_turbs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20302 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/bespoke/place_turbines.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/bespoke/plotting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.793008 NREL-reV-0.8.7/reV/config/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/base_analysis_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/cli_project_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/curtailment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/output_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    36895 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/project_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/config/sam_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.797008 NREL-reV-0.8.7/reV/econ/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/econ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/econ/cli_econ.py
--rw-r--r--   0 runner    (1001) docker     (127)    22544 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/econ/econ.py
--rw-r--r--   0 runner    (1001) docker     (127)     9485 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/econ/economies_of_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/econ/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.797008 NREL-reV-0.8.7/reV/generation/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46673 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/generation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/generation/cli_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    44624 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/generation/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.797008 NREL-reV-0.8.7/reV/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/handlers/cli_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/handlers/cli_multi_year.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/handlers/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29732 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/handlers/multi_year.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/handlers/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/handlers/transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.797008 NREL-reV-0.8.7/reV/hybrids/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/hybrids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/hybrids/cli_hybrids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/hybrids/hybrid_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    45240 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/hybrids/hybrids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.797008 NREL-reV-0.8.7/reV/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45148 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/losses/power_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    26452 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/losses/scheduled.py
--rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.801008 NREL-reV-0.8.7/reV/nrwal/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/nrwal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/nrwal/cli_nrwal.py
--rw-r--r--   0 runner    (1001) docker     (127)    35592 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/nrwal/nrwal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.801008 NREL-reV-0.8.7/reV/qa_qc/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/qa_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/qa_qc/cli_qa_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/qa_qc/qa_qc.py
--rw-r--r--   0 runner    (1001) docker     (127)    30229 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/qa_qc/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.801008 NREL-reV-0.8.7/reV/rep_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/rep_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/rep_profiles/cli_rep_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    46956 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/rep_profiles/rep_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.801008 NREL-reV-0.8.7/reV/supply_curve/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/cli_sc_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/cli_supply_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/competitive_wind_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)    40002 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/extent.py
--rw-r--r--   0 runner    (1001) docker     (127)    78986 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/points.py
--rw-r--r--   0 runner    (1001) docker     (127)    61926 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/sc_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    64830 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/supply_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/supply_curve/tech_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:57:19.801008 NREL-reV-0.8.7/reV/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/utilities/cli_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/utilities/curtailment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/utilities/pytest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/utilities/slots.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/reV/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 18:57:19.805008 NREL-reV-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-03-07 18:57:03.000000 NREL-reV-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.522134 NREL-reV-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-30 19:49:52.000000 NREL-reV-0.8.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.510134 NREL-reV-0.8.9/NREL_reV.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-05-30 19:50:04.000000 NREL-reV-0.8.9/NREL_reV.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-30 19:50:04.000000 NREL-reV-0.8.9/NREL_reV.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:50:04.000000 NREL-reV-0.8.9/NREL_reV.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-30 19:50:04.000000 NREL-reV-0.8.9/NREL_reV.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:50:04.000000 NREL-reV-0.8.9/NREL_reV.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 19:50:04.000000 NREL-reV-0.8.9/NREL_reV.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 19:50:04.000000 NREL-reV-0.8.9/NREL_reV.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-05-30 19:50:04.522134 NREL-reV-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-05-30 19:49:52.000000 NREL-reV-0.8.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.510134 NREL-reV-0.8.9/reV/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.510134 NREL-reV-0.8.9/reV/SAM/
+-rw-r--r--   0 runner    (1001) docker     (127)    30332 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/SAM/SAM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/SAM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/SAM/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20704 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/SAM/econ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87525 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/SAM/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/SAM/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/SAM/windbos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.510134 NREL-reV-0.8.9/reV/bespoke/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/bespoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103328 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/bespoke/bespoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/bespoke/cli_bespoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/bespoke/gradient_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/bespoke/pack_turbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20349 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/bespoke/place_turbines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/bespoke/plotting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.514134 NREL-reV-0.8.9/reV/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/base_analysis_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/cli_project_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/curtailment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/output_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37857 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/project_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/config/sam_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.514134 NREL-reV-0.8.9/reV/econ/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/econ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/econ/cli_econ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22987 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/econ/econ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/econ/economies_of_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/econ/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.514134 NREL-reV-0.8.9/reV/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47943 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/generation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/generation/cli_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45389 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/generation/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.514134 NREL-reV-0.8.9/reV/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/handlers/cli_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/handlers/cli_multi_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/handlers/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29710 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/handlers/multi_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/handlers/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/handlers/transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.514134 NREL-reV-0.8.9/reV/hybrids/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/hybrids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/hybrids/cli_hybrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/hybrids/hybrid_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46590 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/hybrids/hybrids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.518134 NREL-reV-0.8.9/reV/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45148 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/losses/power_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26452 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/losses/scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.518134 NREL-reV-0.8.9/reV/nrwal/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/nrwal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/nrwal/cli_nrwal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36949 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/nrwal/nrwal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.518134 NREL-reV-0.8.9/reV/qa_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/qa_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/qa_qc/cli_qa_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/qa_qc/qa_qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31255 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/qa_qc/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.518134 NREL-reV-0.8.9/reV/rep_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/rep_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/rep_profiles/cli_rep_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48245 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/rep_profiles/rep_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.518134 NREL-reV-0.8.9/reV/supply_curve/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38752 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/cli_sc_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/cli_supply_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/competitive_wind_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42949 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81669 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63039 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/sc_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66599 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/supply_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/supply_curve/tech_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:50:04.522134 NREL-reV-0.8.9/reV/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/utilities/cli_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/utilities/curtailment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/utilities/pytest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/utilities/slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/reV/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:50:04.522134 NREL-reV-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-30 19:49:53.000000 NREL-reV-0.8.9/setup.py
```

### Comparing `NREL-reV-0.8.7/LICENSE` & `NREL-reV-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/NREL_reV.egg-info/PKG-INFO` & `NREL-reV-0.8.9/NREL_reV.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: NREL-reV
-Version: 0.8.7
+Version: 0.8.9
 Summary: National Renewable Energy Laboratory's (NREL's) Renewable Energy Potential(V) Model: reV
 Home-page: https://nrel.github.io/reV/
 Author: Galen Maclaurin
 Author-email: galen.maclaurin@nrel.gov
 License: BSD 3-Clause
 Description: 
                 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
         
         
-        .. image:: https://github.com/NREL/reV/workflows/Documentation/badge.svg
+        |Docs| |Tests| |Linter| |PythonV| |Pypi| |Codecov| |Zenodo| |Binder|
+        
+        .. |Docs| image:: https://github.com/NREL/reV/workflows/Documentation/badge.svg
             :target: https://nrel.github.io/reV/
         
-        .. image:: https://github.com/NREL/reV/workflows/Pytests/badge.svg
+        .. |Tests| image:: https://github.com/NREL/reV/workflows/Pytests/badge.svg
             :target: https://github.com/NREL/reV/actions?query=workflow%3A%22Pytests%22
         
-        .. image:: https://github.com/NREL/reV/workflows/Lint%20Code%20Base/badge.svg
+        .. |Linter| image:: https://github.com/NREL/reV/workflows/Lint%20Code%20Base/badge.svg
             :target: https://github.com/NREL/reV/actions?query=workflow%3A%22Lint+Code+Base%22
         
-        .. image:: https://img.shields.io/pypi/pyversions/NREL-reV.svg
+        .. |PythonV| image:: https://img.shields.io/pypi/pyversions/NREL-reV.svg
             :target: https://pypi.org/project/NREL-reV/
         
-        .. image:: https://badge.fury.io/py/NREL-reV.svg
+        .. |Pypi| image:: https://badge.fury.io/py/NREL-reV.svg
             :target: https://badge.fury.io/py/NREL-reV
         
-        .. image:: https://codecov.io/gh/nrel/reV/branch/main/graph/badge.svg?token=U4ZU9F0K0Z
+        .. |Codecov| image:: https://codecov.io/gh/nrel/reV/branch/main/graph/badge.svg?token=U4ZU9F0K0Z
             :target: https://codecov.io/gh/nrel/reV
         
-        .. image:: https://zenodo.org/badge/201343076.svg
+        .. |Zenodo| image:: https://zenodo.org/badge/201343076.svg
            :target: https://zenodo.org/badge/latestdoi/201343076
         
-        .. image:: https://mybinder.org/badge_logo.svg
+        .. |Binder| image:: https://mybinder.org/badge_logo.svg
             :target: https://mybinder.org/v2/gh/nrel/reV/HEAD
         
         |
         
         .. inclusion-intro
         
         **reV** (the Renewable Energy Potential model)
```

### Comparing `NREL-reV-0.8.7/NREL_reV.egg-info/SOURCES.txt` & `NREL-reV-0.8.9/NREL_reV.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/NREL_reV.egg-info/entry_points.txt` & `NREL-reV-0.8.9/NREL_reV.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/PKG-INFO` & `NREL-reV-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: NREL-reV
-Version: 0.8.7
+Version: 0.8.9
 Summary: National Renewable Energy Laboratory's (NREL's) Renewable Energy Potential(V) Model: reV
 Home-page: https://nrel.github.io/reV/
 Author: Galen Maclaurin
 Author-email: galen.maclaurin@nrel.gov
 License: BSD 3-Clause
 Description: 
                 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
         
         
-        .. image:: https://github.com/NREL/reV/workflows/Documentation/badge.svg
+        |Docs| |Tests| |Linter| |PythonV| |Pypi| |Codecov| |Zenodo| |Binder|
+        
+        .. |Docs| image:: https://github.com/NREL/reV/workflows/Documentation/badge.svg
             :target: https://nrel.github.io/reV/
         
-        .. image:: https://github.com/NREL/reV/workflows/Pytests/badge.svg
+        .. |Tests| image:: https://github.com/NREL/reV/workflows/Pytests/badge.svg
             :target: https://github.com/NREL/reV/actions?query=workflow%3A%22Pytests%22
         
-        .. image:: https://github.com/NREL/reV/workflows/Lint%20Code%20Base/badge.svg
+        .. |Linter| image:: https://github.com/NREL/reV/workflows/Lint%20Code%20Base/badge.svg
             :target: https://github.com/NREL/reV/actions?query=workflow%3A%22Lint+Code+Base%22
         
-        .. image:: https://img.shields.io/pypi/pyversions/NREL-reV.svg
+        .. |PythonV| image:: https://img.shields.io/pypi/pyversions/NREL-reV.svg
             :target: https://pypi.org/project/NREL-reV/
         
-        .. image:: https://badge.fury.io/py/NREL-reV.svg
+        .. |Pypi| image:: https://badge.fury.io/py/NREL-reV.svg
             :target: https://badge.fury.io/py/NREL-reV
         
-        .. image:: https://codecov.io/gh/nrel/reV/branch/main/graph/badge.svg?token=U4ZU9F0K0Z
+        .. |Codecov| image:: https://codecov.io/gh/nrel/reV/branch/main/graph/badge.svg?token=U4ZU9F0K0Z
             :target: https://codecov.io/gh/nrel/reV
         
-        .. image:: https://zenodo.org/badge/201343076.svg
+        .. |Zenodo| image:: https://zenodo.org/badge/201343076.svg
            :target: https://zenodo.org/badge/latestdoi/201343076
         
-        .. image:: https://mybinder.org/badge_logo.svg
+        .. |Binder| image:: https://mybinder.org/badge_logo.svg
             :target: https://mybinder.org/v2/gh/nrel/reV/HEAD
         
         |
         
         .. inclusion-intro
         
         **reV** (the Renewable Energy Potential model)
```

### Comparing `NREL-reV-0.8.7/README.rst` & `NREL-reV-0.8.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,38 @@
         <img height="180" src="docs/source/_static/logo.png" />
         &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
         <img height="170" src="docs/source/_static/RD100_2023_Winner_Logo.png" />
     </p>
 
 ---------
 
-.. image:: https://github.com/NREL/reV/workflows/Documentation/badge.svg
+|Docs| |Tests| |Linter| |PythonV| |Pypi| |Codecov| |Zenodo| |Binder|
+
+.. |Docs| image:: https://github.com/NREL/reV/workflows/Documentation/badge.svg
     :target: https://nrel.github.io/reV/
 
-.. image:: https://github.com/NREL/reV/workflows/Pytests/badge.svg
+.. |Tests| image:: https://github.com/NREL/reV/workflows/Pytests/badge.svg
     :target: https://github.com/NREL/reV/actions?query=workflow%3A%22Pytests%22
 
-.. image:: https://github.com/NREL/reV/workflows/Lint%20Code%20Base/badge.svg
+.. |Linter| image:: https://github.com/NREL/reV/workflows/Lint%20Code%20Base/badge.svg
     :target: https://github.com/NREL/reV/actions?query=workflow%3A%22Lint+Code+Base%22
 
-.. image:: https://img.shields.io/pypi/pyversions/NREL-reV.svg
+.. |PythonV| image:: https://img.shields.io/pypi/pyversions/NREL-reV.svg
     :target: https://pypi.org/project/NREL-reV/
 
-.. image:: https://badge.fury.io/py/NREL-reV.svg
+.. |Pypi| image:: https://badge.fury.io/py/NREL-reV.svg
     :target: https://badge.fury.io/py/NREL-reV
 
-.. image:: https://codecov.io/gh/nrel/reV/branch/main/graph/badge.svg?token=U4ZU9F0K0Z
+.. |Codecov| image:: https://codecov.io/gh/nrel/reV/branch/main/graph/badge.svg?token=U4ZU9F0K0Z
     :target: https://codecov.io/gh/nrel/reV
 
-.. image:: https://zenodo.org/badge/201343076.svg
+.. |Zenodo| image:: https://zenodo.org/badge/201343076.svg
    :target: https://zenodo.org/badge/latestdoi/201343076
 
-.. image:: https://mybinder.org/badge_logo.svg
+.. |Binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/nrel/reV/HEAD
 
 |
 
 .. inclusion-intro
 
 **reV** (the Renewable Energy Potential model)
```

### Comparing `NREL-reV-0.8.7/reV/SAM/SAM.py` & `NREL-reV-0.8.9/reV/SAM/SAM.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,66 @@
 # -*- coding: utf-8 -*-
 """reV-to-SAM interface module.
 
 Wraps the NREL-PySAM library with additional reV features.
 """
+
 import copy
 import json
 import logging
-import numpy as np
 import os
-import pandas as pd
 from warnings import warn
-import PySAM.GenericSystem as generic
-
-from reV.utilities.exceptions import (SAMInputWarning, SAMInputError,
-                                      SAMExecutionError, ResourceError)
 
-from rex.multi_file_resource import (MultiFileResource, MultiFileNSRDB,
-                                     MultiFileWTK)
-from rex.renewable_resource import (WindResource, SolarResource, NSRDB,
-                                    WaveResource, GeothermalResource)
+import numpy as np
+import pandas as pd
+import PySAM.GenericSystem as generic
+from rex.multi_file_resource import (
+    MultiFileNSRDB,
+    MultiFileResource,
+    MultiFileWTK,
+)
 from rex.multi_res_resource import MultiResolutionResource
+from rex.renewable_resource import (
+    NSRDB,
+    GeothermalResource,
+    SolarResource,
+    WaveResource,
+    WindResource,
+)
 from rex.utilities.utilities import check_res_file
 
+from reV.utilities import ResourceMetaField
+from reV.utilities.exceptions import (
+    ResourceError,
+    SAMExecutionError,
+    SAMInputError,
+    SAMInputWarning,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class SamResourceRetriever:
     """Factory utility to get the SAM resource handler."""
 
     # Mapping for reV technology and SAM module to h5 resource handler type
     # SolarResource is swapped for NSRDB if the res_file contains "nsrdb"
-    RESOURCE_TYPES = {'geothermal': GeothermalResource,
-                      'pvwattsv5': SolarResource,
-                      'pvwattsv7': SolarResource,
-                      'pvwattsv8': SolarResource,
-                      'pvsamv1': SolarResource,
-                      'tcsmoltensalt': SolarResource,
-                      'solarwaterheat': SolarResource,
-                      'troughphysicalheat': SolarResource,
-                      'lineardirectsteam': SolarResource,
-                      'windpower': WindResource,
-                      'mhkwave': WaveResource
-                      }
+    RESOURCE_TYPES = {
+        "geothermal": GeothermalResource,
+        "pvwattsv5": SolarResource,
+        "pvwattsv7": SolarResource,
+        "pvwattsv8": SolarResource,
+        "pvsamv1": SolarResource,
+        "tcsmoltensalt": SolarResource,
+        "solarwaterheat": SolarResource,
+        "troughphysicalheat": SolarResource,
+        "lineardirectsteam": SolarResource,
+        "windpower": WindResource,
+        "mhkwave": WaveResource,
+    }
 
     @staticmethod
     def _get_base_handler(res_file, module):
         """Get the base SAM resource handler, raise error if module not found.
 
         Parameters
         ----------
@@ -65,23 +79,25 @@
             Solar or Wind resource handler based on input.
         """
 
         try:
             res_handler = SamResourceRetriever.RESOURCE_TYPES[module.lower()]
 
         except KeyError as e:
-            msg = ('Cannot interpret what kind of resource handler the SAM '
-                   'module or reV technology "{}" requires. Expecting one of '
-                   'the following SAM modules or reV technologies: {}'
-                   .format(module,
-                           list(SamResourceRetriever.RESOURCE_TYPES.keys())))
+            msg = (
+                "Cannot interpret what kind of resource handler the SAM "
+                'module or reV technology "{}" requires. Expecting one of '
+                "the following SAM modules or reV technologies: {}".format(
+                    module, list(SamResourceRetriever.RESOURCE_TYPES.keys())
+                )
+            )
             logger.exception(msg)
             raise SAMExecutionError(msg) from e
 
-        if res_handler == SolarResource and 'nsrdb' in res_file.lower():
+        if res_handler == SolarResource and "nsrdb" in res_file.lower():
             # Use NSRDB handler if definitely an NSRDB file
             res_handler = NSRDB
 
         return res_handler
 
     @staticmethod
     def _parse_gid_map_sites(gen_gids, gid_map=None):
@@ -109,16 +125,17 @@
         if gid_map is None:
             res_gids = gen_gids
         else:
             res_gids = [gid_map[i] for i in gen_gids]
         return res_gids
 
     @classmethod
-    def _make_res_kwargs(cls, res_handler, project_points, output_request,
-                         gid_map):
+    def _make_res_kwargs(
+        cls, res_handler, project_points, output_request, gid_map
+    ):
         """
         Make Resource.preloadSam args and kwargs
 
         Parameters
         ----------
         res_handler : Resource handler
             Wind resource handler.
@@ -142,48 +159,52 @@
         """
         sites = cls._parse_gid_map_sites(project_points.sites, gid_map=gid_map)
         args = (sites,)
 
         kwargs = {}
         if res_handler in (SolarResource, NSRDB):
             # check for clearsky irradiation analysis for NSRDB
-            kwargs['clearsky'] = project_points.sam_config_obj.clearsky
-            kwargs['bifacial'] = project_points.sam_config_obj.bifacial
-            kwargs['tech'] = project_points.tech
+            kwargs["clearsky"] = project_points.sam_config_obj.clearsky
+            kwargs["bifacial"] = project_points.sam_config_obj.bifacial
+            kwargs["tech"] = project_points.tech
 
             downscale = project_points.sam_config_obj.downscale
             # check for downscaling request
             if downscale is not None:
                 # make sure that downscaling is only requested for NSRDB
                 # resource
                 if res_handler != NSRDB:
-                    msg = ('Downscaling was requested for a non-NSRDB '
-                           'resource file. reV does not have this capability '
-                           'at the current time. Please contact a developer '
-                           'for more information on this feature.')
+                    msg = (
+                        "Downscaling was requested for a non-NSRDB "
+                        "resource file. reV does not have this capability "
+                        "at the current time. Please contact a developer "
+                        "for more information on this feature."
+                    )
                     logger.warning(msg)
                     warn(msg, SAMInputWarning)
                 else:
                     # pass through the downscaling request
-                    kwargs['downscale'] = downscale
+                    kwargs["downscale"] = downscale
 
         elif res_handler == WindResource:
-            args += (project_points.h, )
-            kwargs['icing'] = project_points.sam_config_obj.icing
-            if project_points.curtailment is not None:
-                if project_points.curtailment.precipitation:
-                    # make precip rate available for curtailment analysis
-                    kwargs['precip_rate'] = True
+            args += (project_points.h,)
+            kwargs["icing"] = project_points.sam_config_obj.icing
+            if (
+                project_points.curtailment is not None
+                and project_points.curtailment.precipitation
+            ):
+                # make precip rate available for curtailment analysis
+                kwargs["precip_rate"] = True
 
         elif res_handler == GeothermalResource:
-            args += (project_points.d, )
+            args += (project_points.d,)
 
         # Check for resource means
-        if any(req.endswith('_mean') for req in output_request):
-            kwargs['means'] = True
+        if any(req.endswith("_mean") for req in output_request):
+            kwargs["means"] = True
 
         return kwargs, args
 
     @staticmethod
     def _multi_file_mods(res_handler, kwargs, res_file):
         """
         Check if res_file is a multi-file resource dir and update handler
@@ -214,17 +235,25 @@
             res_handler = MultiFileNSRDB
         else:
             res_handler = MultiFileResource
 
         return res_handler, kwargs, res_file
 
     @classmethod
-    def get(cls, res_file, project_points, module,
-            output_request=('cf_mean', ), gid_map=None,
-            lr_res_file=None, nn_map=None, bias_correct=None):
+    def get(
+        cls,
+        res_file,
+        project_points,
+        module,
+        output_request=("cf_mean",),
+        gid_map=None,
+        lr_res_file=None,
+        nn_map=None,
+        bias_correct=None,
+    ):
         """Get the SAM resource iterator object (single year, single file).
 
         Parameters
         ----------
         res_file : str
             Single resource file (with full path) to retrieve.
         project_points : reV.config.ProjectPoints
@@ -276,58 +305,61 @@
         Returns
         -------
         res : reV.resource.SAMResource
             Resource iterator object to pass to SAM.
         """
 
         res_handler = cls._get_base_handler(res_file, module)
-        kwargs, args = cls._make_res_kwargs(res_handler, project_points,
-                                            output_request, gid_map)
+        kwargs, args = cls._make_res_kwargs(
+            res_handler, project_points, output_request, gid_map
+        )
 
         multi_h5_res, hsds = check_res_file(res_file)
         if multi_h5_res:
-            res_handler, kwargs, res_file = cls._multi_file_mods(res_handler,
-                                                                 kwargs,
-                                                                 res_file)
+            res_handler, kwargs, res_file = cls._multi_file_mods(
+                res_handler, kwargs, res_file
+            )
         else:
-            kwargs['hsds'] = hsds
+            kwargs["hsds"] = hsds
 
-        kwargs['time_index_step'] = \
+        kwargs["time_index_step"] = (
             project_points.sam_config_obj.time_index_step
+        )
 
         if lr_res_file is None:
             res = res_handler.preload_SAM(res_file, *args, **kwargs)
         else:
-            kwargs['handler_class'] = res_handler
-            kwargs['nn_map'] = nn_map
-            res = MultiResolutionResource.preload_SAM(res_file, lr_res_file,
-                                                      *args, **kwargs)
+            kwargs["handler_class"] = res_handler
+            kwargs["nn_map"] = nn_map
+            res = MultiResolutionResource.preload_SAM(
+                res_file, lr_res_file, *args, **kwargs
+            )
 
         if bias_correct is not None:
             res.bias_correct(bias_correct)
 
         return res
 
 
 class Sam:
     """reV wrapper on the PySAM framework."""
 
     # PySAM object wrapped by this class
     PYSAM = generic
 
     # callable attributes to be ignored in the get/set logic
-    IGNORE_ATTRS = ['assign', 'execute', 'export']
+    IGNORE_ATTRS = ["assign", "execute", "export"]
 
     def __init__(self):
         self._pysam = self.PYSAM.new()
         self._attr_dict = None
         self._inputs = []
         self.sam_sys_inputs = {}
-        if 'constant' in self.input_list:
-            self['constant'] = 0.0
+        if "constant" in self.input_list:
+            self["constant"] = 0.0
 
     def __getitem__(self, key):
         """Get the value of a PySAM attribute (either input or output).
 
         Parameters
         ----------
         key : str
@@ -355,47 +387,50 @@
         key : str
             Lowest level attribute name.
         value : object
             Data to set to the key.
         """
 
         if key not in self.input_list:
-            msg = ('Could not set input key "{}". Attribute not '
-                   'found in PySAM object: "{}"'
-                   .format(key, self.pysam))
+            msg = (
+                'Could not set input key "{}". Attribute not '
+                'found in PySAM object: "{}"'.format(key, self.pysam)
+            )
             logger.exception(msg)
             raise SAMInputError(msg)
-        else:
-            self.sam_sys_inputs[key] = value
-            group = self._get_group(key, outputs=False)
-            try:
-                setattr(getattr(self.pysam, group), key, value)
-            except Exception as e:
-                msg = ('Could not set input key "{}" to '
-                       'group "{}" in "{}".\n'
-                       'Data is: {} ({})\n'
-                       'Received the following error: "{}"'
-                       .format(key, group, self.pysam, value, type(value), e))
-                logger.exception(msg)
-                raise SAMInputError(msg) from e
+        self.sam_sys_inputs[key] = value
+        group = self._get_group(key, outputs=False)
+        try:
+            setattr(getattr(self.pysam, group), key, value)
+        except Exception as e:
+            msg = (
+                'Could not set input key "{}" to '
+                'group "{}" in "{}".\n'
+                "Data is: {} ({})\n"
+                'Received the following error: "{}"'.format(
+                    key, group, self.pysam, value, type(value), e
+                )
+            )
+            logger.exception(msg)
+            raise SAMInputError(msg) from e
 
     @property
     def pysam(self):
         """Get the pysam object."""
         return self._pysam
 
     @classmethod
     def default(cls):
         """Get the executed default pysam object.
 
         Returns
         -------
         PySAM.GenericSystem
         """
-        obj = cls.PYSAM.default('GenericSystemNone')
+        obj = cls.PYSAM.default("GenericSystemNone")
         obj.execute()
 
         return obj
 
     @property
     def attr_dict(self):
         """Get the heirarchical PySAM object attribute dictionary.
@@ -405,31 +440,32 @@
         _attr_dict : dict
             Dictionary with:
                keys: variable groups
                values: lowest level attribute/variable names
         """
         if self._attr_dict is None:
             keys = self._get_pysam_attrs(self.pysam)
-            self._attr_dict = {k: self._get_pysam_attrs(getattr(self.pysam, k))
-                               for k in keys}
+            self._attr_dict = {
+                k: self._get_pysam_attrs(getattr(self.pysam, k)) for k in keys
+            }
 
         return self._attr_dict
 
     @property
     def input_list(self):
         """Get the list of lowest level input attribute/variable names.
 
         Returns
         -------
         _inputs : list
             List of lowest level input attributes.
         """
         if not any(self._inputs):
             for k, v in self.attr_dict.items():
-                if k.lower() != 'outputs':
+                if k.lower() != "outputs":
                     self._inputs += v
 
         return self._inputs
 
     def _get_group(self, key, outputs=True):
         """Get the group that the input key belongs to.
 
@@ -446,16 +482,15 @@
         group : str | None
             PySAM attribute group that key belongs to. None if not found.
         """
         group = None
 
         temp = self.attr_dict
         if not outputs:
-            temp = {k: v for (k, v) in temp.items()
-                    if k.lower() != 'outputs'}
+            temp = {k: v for (k, v) in temp.items() if k.lower() != "outputs"}
 
         for k, v in temp.items():
             if key in v:
                 group = k
                 break
 
         return group
@@ -470,16 +505,19 @@
 
         Returns
         -------
         attrs : list
             List of attrs belonging to obj with dunder attrs and IGNORE_ATTRS
             not included.
         """
-        attrs = [a for a in dir(obj) if not a.startswith('__')
-                 and a not in self.IGNORE_ATTRS]
+        attrs = [
+            a
+            for a in dir(obj)
+            if not a.startswith("__") and a not in self.IGNORE_ATTRS
+        ]
         return attrs
 
     def execute(self):
         """Call the PySAM execute method. Raise SAMExecutionError if error."""
         try:
             self.pysam.execute()
         except Exception as e:
@@ -502,27 +540,29 @@
         -------
         key : str
             Filtered SAM input key.
         value : str | int | float | list | np.ndarray
             Filtered Input value associated with key.
         """
 
-        if '.' in key:
-            key = key.replace('.', '_')
+        if "." in key:
+            key = key.replace(".", "_")
 
-        if ':constant' in key and 'adjust:' in key:
-            key = key.replace('adjust:', '')
+        if ":constant" in key and "adjust:" in key:
+            key = key.replace("adjust:", "")
 
-        if isinstance(value, str) and '[' in value and ']' in value:
+        if isinstance(value, str) and "[" in value and "]" in value:
             try:
                 value = json.loads(value)
             except json.JSONDecodeError:
-                msg = ('Found a weird SAM config input for "{}" that looks '
-                       'like a stringified-list but could not run through '
-                       'json.loads() so skipping: {}'.format(key, value))
+                msg = (
+                    'Found a weird SAM config input for "{}" that looks '
+                    "like a stringified-list but could not run through "
+                    "json.loads() so skipping: {}".format(key, value)
+                )
                 logger.warning(msg)
                 warn(msg)
 
         return key, value
 
     def assign_inputs(self, inputs, raise_warning=False):
         """Assign a flat dictionary of inputs to the PySAM object.
@@ -537,41 +577,41 @@
         """
 
         for k, v in inputs.items():
             k, v = self._filter_inputs(k, v)
             if k in self.input_list and v is not None:
                 self[k] = v
             elif raise_warning:
-                wmsg = ('Not setting input "{}" to: {}.'
-                        .format(k, v))
+                wmsg = 'Not setting input "{}" to: {}.'.format(k, v)
                 warn(wmsg, SAMInputWarning)
                 logger.warning(wmsg)
 
 
 class RevPySam(Sam):
     """Base class for reV-SAM simulations (generation and econ)."""
 
     DIR = os.path.dirname(os.path.realpath(__file__))
     MODULE = None
 
-    def __init__(self, meta, sam_sys_inputs, output_request,
-                 site_sys_inputs=None):
+    def __init__(
+        self, meta, sam_sys_inputs, output_request, site_sys_inputs=None
+    ):
         """Initialize a SAM object.
 
         Parameters
         ----------
         meta : pd.DataFrame | pd.Series | None
             Meta data corresponding to the resource input for the single
             location. Should include values for latitude, longitude, elevation,
             and timezone. Can be None for econ runs.
         sam_sys_inputs : dict
             Site-agnostic SAM system model inputs arguments.
         output_request : list
             Requested SAM outputs (e.g., 'cf_mean', 'annual_energy',
-            'cf_profile', 'gen_profile', 'energy_yield', 'ppa_price',
+            , 'gen_profile', 'energy_yield', 'ppa_price',
             'lcoe_fcr').
         site_sys_inputs : dict
             Optional set of site-specific SAM system inputs to complement the
             site-agnostic inputs.
         """
 
         super().__init__()
@@ -619,19 +659,21 @@
 
         Returns
         -------
         resource : pd.DataFrame
             Resource dataframe with all February 29th timesteps removed.
         """
 
-        if hasattr(resource, 'index'):
-            if (hasattr(resource.index, 'month')
-                    and hasattr(resource.index, 'day')):
-                leap_day = ((resource.index.month == 2)
-                            & (resource.index.day == 29))
+        if hasattr(resource, "index"):
+            if hasattr(resource.index, "month") and hasattr(
+                resource.index, "day"
+            ):
+                leap_day = (resource.index.month == 2) & (
+                    resource.index.day == 29
+                )
                 resource = resource.drop(resource.index[leap_day])
 
         return resource
 
     @staticmethod
     def ensure_res_len(arr, time_index):
         """
@@ -647,42 +689,46 @@
             frequency and number of days
 
         Returns
         -------
         arr : ndarray
             Truncated array of data such that there are 365 days
         """
-        msg = ('A valid time_index must be supplied to ensure the proper '
-               'resource length! Instead {} was supplied'
-               .format(type(time_index)))
+        msg = (
+            "A valid time_index must be supplied to ensure the proper "
+            "resource length! Instead {} was supplied".format(type(time_index))
+        )
         assert isinstance(time_index, pd.DatetimeIndex)
 
-        msg = ('arr length {} does not match time_index length {}!'
-               .format(len(arr), len(time_index)))
+        msg = "arr length {} does not match time_index length {}!".format(
+            len(arr), len(time_index)
+        )
         assert len(arr) == len(time_index)
 
         if time_index.is_leap_year.all():
             mask = time_index.month == 2
             mask &= time_index.day == 29
             if not mask.any():
                 mask = time_index.month == 2
                 mask &= time_index.day == 28
                 s = np.where(mask)[0][-1]
 
                 freq = pd.infer_freq(time_index[:s])
-                msg = 'frequencies do not match before and after 2/29'
+                msg = "frequencies do not match before and after 2/29"
                 assert freq == pd.infer_freq(time_index[s + 1:]), msg
             else:
                 freq = pd.infer_freq(time_index)
         else:
             freq = pd.infer_freq(time_index)
 
         if freq is None:
-            msg = ('Resource time_index does not have a consistent time-step '
-                   '(frequency)!')
+            msg = (
+                "Resource time_index does not have a consistent time-step "
+                "(frequency)!"
+            )
             logger.error(msg)
             raise ResourceError(msg)
 
         doy = time_index.dayofyear
         n_doy = len(doy.unique())
 
         if n_doy > 365:
@@ -692,15 +738,15 @@
             arr = arr[mask]
 
         return arr
 
     @staticmethod
     def make_datetime(series):
         """Ensure that pd series is a datetime series with dt accessor"""
-        if not hasattr(series, 'dt'):
+        if not hasattr(series, "dt"):
             series = pd.to_datetime(pd.Series(series))
 
         return series
 
     @classmethod
     def get_time_interval(cls, time_index):
         """Get the time interval.
@@ -723,15 +769,15 @@
         time_interval = 0
 
         # iterate through the hourly time diffs and count indices between flips
         for t in x[1:]:
             if t == 1.0:
                 time_interval += 1
                 break
-            elif t == 0.0:
+            if t == 0.0:
                 time_interval += 1
 
         return int(time_interval)
 
     @staticmethod
     def _parse_meta(meta):
         """Make sure the meta data corresponds to a single location and convert
@@ -747,18 +793,19 @@
         Parameters
         ----------
         meta : pd.Series | None
             Meta data corresponding to the resource input for the single
             location. Should include values for latitude, longitude, elevation,
             and timezone. Can be None for econ runs.
         """
-
         if isinstance(meta, pd.DataFrame):
-            msg = ('Meta data must only be for a single site but received: {}'
-                   .format(meta))
+            msg = (
+                "Meta data must only be for a single site but received: "
+                f"{meta}"
+            )
             assert len(meta) == 1, msg
             meta = meta.iloc[0]
 
         if meta is not None:
             assert isinstance(meta, pd.Series)
 
         return meta
@@ -781,46 +828,47 @@
                     self.sam_sys_inputs[k] = v
 
     @staticmethod
     def _is_arr_like(val):
         """Returns true if SAM data is array-like. False if scalar."""
         if isinstance(val, (int, float, str)):
             return False
+        try:
+            len(val)
+        except TypeError:
+            return False
         else:
-            try:
-                len(val)
-            except TypeError:
-                return False
-            else:
-                return True
+            return True
 
     @classmethod
     def _is_hourly(cls, val):
         """Returns true if SAM data is hourly or sub-hourly. False otherise."""
         if not cls._is_arr_like(val):
             return False
-        else:
-            L = len(val)
-            return L >= 8760
+        L = len(val)
+        return L >= 8760
 
     def outputs_to_utc_arr(self):
         """Convert array-like SAM outputs to UTC np.ndarrays"""
         if self.outputs is not None:
             for key, output in self.outputs.items():
                 if self._is_arr_like(output):
                     output = np.asarray(output)
 
                     if output.dtype == np.float64:
                         output = output.astype(np.float32)
                     elif output.dtype == np.int64:
                         output = output.astype(np.int32)
 
                     if self._is_hourly(output):
-                        n_roll = int(-1 * self.meta['timezone']
-                                     * self.time_interval)
+                        n_roll = int(
+                            -1
+                            * self.meta[ResourceMetaField.TIMEZONE]
+                            * self.time_interval
+                        )
                         output = np.roll(output, n_roll)
 
                     self.outputs[key] = output
 
     def collect_outputs(self, output_lookup):
         """Collect SAM output_request, convert timeseries outputs to UTC, and
         save outputs to self.outputs property.
@@ -857,13 +905,14 @@
     def execute(self):
         """Call the PySAM execute method. Raise SAMExecutionError if error.
         Include the site index if available.
         """
         try:
             self.pysam.execute()
         except Exception as e:
-            msg = ('PySAM raised an error while executing: "{}"'
-                   .format(self.module))
+            msg = 'PySAM raised an error while executing: "{}"'.format(
+                self.module
+            )
             if self.site is not None:
-                msg += ' for site {}'.format(self.site)
+                msg += " for site {}".format(self.site)
             logger.exception(msg)
             raise SAMExecutionError(msg) from e
```

### Comparing `NREL-reV-0.8.7/reV/SAM/defaults.py` & `NREL-reV-0.8.9/reV/SAM/defaults.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/SAM/econ.py` & `NREL-reV-0.8.9/reV/SAM/econ.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # -*- coding: utf-8 -*-
 """reV-to-SAM econ interface module.
 
 Wraps the NREL-PySAM lcoefcr and singleowner modules with
 additional reV features.
 """
-from copy import deepcopy
 import logging
-import numpy as np
+from copy import deepcopy
 from warnings import warn
+
+import numpy as np
 import PySAM.Lcoefcr as PySamLCOE
 import PySAM.Singleowner as PySamSingleOwner
 
-from reV.SAM.defaults import DefaultSingleOwner, DefaultLCOE
 from reV.handlers.outputs import Outputs
-from reV.SAM.windbos import WindBos
+from reV.SAM.defaults import DefaultLCOE, DefaultSingleOwner
 from reV.SAM.SAM import RevPySam
+from reV.SAM.windbos import WindBos
 from reV.utilities.exceptions import SAMExecutionError
+from reV.utilities import ResourceMetaField
 
 logger = logging.getLogger(__name__)
 
 
 class Economic(RevPySam):
     """Base class for SAM economic models."""
+
     MODULE = None
 
     def __init__(self, sam_sys_inputs, site_sys_inputs=None,
                  output_request='lcoe_fcr'):
         """Initialize a SAM economic model object.
 
         Parameters
@@ -168,15 +171,15 @@
             the requested sites.
         """
 
         # Retrieve the generation profile for single owner input
         with Outputs(cf_file) as cfh:
 
             # get the index location of the site in question
-            site_gids = list(cfh.get_meta_arr('gid'))
+            site_gids = list(cfh.get_meta_arr(ResourceMetaField.GID))
             isites = [site_gids.index(s) for s in sites]
 
             # look for the cf_profile dataset
             if 'cf_profile' in cfh.datasets:
                 dset = 'cf_profile'
             elif 'cf_profile-{}'.format(year) in cfh.datasets:
                 dset = 'cf_profile-{}'.format(year)
@@ -331,14 +334,15 @@
 
         return sim.outputs
 
 
 class LCOE(Economic):
     """SAM LCOE model.
     """
+
     MODULE = 'lcoefcr'
     PYSAM = PySamLCOE
 
     def __init__(self, sam_sys_inputs, site_sys_inputs=None,
                  output_request=('lcoe_fcr',)):
         """Initialize a SAM LCOE economic model object."""
         super().__init__(sam_sys_inputs, site_sys_inputs=site_sys_inputs,
@@ -371,15 +375,15 @@
         cf_arr : np.ndarray
             Array of cf_mean values for all sites in the cf_file for the
             given year.
         """
 
         # get the cf_file meta data gid's to use as indexing tools
         with Outputs(cf_file) as cfh:
-            site_gids = list(cfh.meta['gid'])
+            site_gids = list(cfh.meta[ResourceMetaField.GID])
 
         calc_aey = False
         if 'annual_energy' not in site_df:
             # annual energy yield has not been input, flag to calculate
             site_df.loc[:, 'annual_energy'] = np.nan
             calc_aey = True
 
@@ -459,14 +463,15 @@
 
         return out
 
 
 class SingleOwner(Economic):
     """SAM single owner economic model.
     """
+
     MODULE = 'singleowner'
     PYSAM = PySamSingleOwner
 
     def __init__(self, sam_sys_inputs, site_sys_inputs=None,
                  output_request=('ppa_price',)):
         """Initialize a SAM single owner economic model object.
         """
@@ -493,22 +498,21 @@
             Dictionary of SAM key-value pair inputs with the total installed
             cost replaced with WindBOS values if requested.
         output : dict
             Dictionary of windbos cost breakdowns.
         """
 
         outputs = {}
-        if inputs is not None:
-            if 'total_installed_cost' in inputs:
-                if isinstance(inputs['total_installed_cost'], str):
-                    if inputs['total_installed_cost'].lower() == 'windbos':
-                        wb = WindBos(inputs)
-                        inputs['total_installed_cost'] = \
-                            wb.total_installed_cost
-                        outputs = wb.output
+        if (inputs is not None
+                and 'total_installed_cost' in inputs
+                and isinstance(inputs['total_installed_cost'], str)
+                and inputs['total_installed_cost'].lower() == 'windbos'):
+            wb = WindBos(inputs)
+            inputs['total_installed_cost'] = wb.total_installed_cost
+            outputs = wb.output
         return inputs, outputs
 
     @staticmethod
     def default():
         """Get the executed default pysam Single Owner object.
 
         Returns
```

### Comparing `NREL-reV-0.8.7/reV/SAM/generation.py` & `NREL-reV-0.8.9/reV/SAM/generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 """reV-to-SAM generation interface module.
 
 Wraps the NREL-PySAM pvwattsv5, windpower, and tcsmolensalt modules with
 additional reV features.
 """
+
 import copy
-import os
 import logging
-
+import os
 from abc import ABC, abstractmethod
 from tempfile import TemporaryDirectory
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 import PySAM.Geothermal as PySamGeothermal
@@ -22,39 +22,52 @@
 import PySAM.Pvwattsv7 as PySamPv7
 import PySAM.Pvwattsv8 as PySamPv8
 import PySAM.Swh as PySamSwh
 import PySAM.TcsmoltenSalt as PySamCSP
 import PySAM.TroughPhysicalProcessHeat as PySamTpph
 import PySAM.Windpower as PySamWindPower
 
-from reV.losses import ScheduledLossesMixin, PowerCurveLossesMixin
-from reV.SAM.defaults import (DefaultGeothermal,
-                              DefaultPvWattsv5,
-                              DefaultPvWattsv8,
-                              DefaultPvSamv1,
-                              DefaultWindPower,
-                              DefaultTcsMoltenSalt,
-                              DefaultSwh,
-                              DefaultTroughPhysicalProcessHeat,
-                              DefaultLinearFresnelDsgIph,
-                              DefaultMhkWave)
+from reV.losses import PowerCurveLossesMixin, ScheduledLossesMixin
+from reV.SAM.defaults import (
+    DefaultGeothermal,
+    DefaultLinearFresnelDsgIph,
+    DefaultMhkWave,
+    DefaultPvSamv1,
+    DefaultPvWattsv5,
+    DefaultPvWattsv8,
+    DefaultSwh,
+    DefaultTcsMoltenSalt,
+    DefaultTroughPhysicalProcessHeat,
+    DefaultWindPower,
+)
 from reV.SAM.econ import LCOE, SingleOwner
 from reV.SAM.SAM import RevPySam
+from reV.utilities import ResourceMetaField, SupplyCurveField
 from reV.utilities.curtailment import curtail
-from reV.utilities.exceptions import (SAMInputWarning, SAMExecutionError,
-                                      InputError)
+from reV.utilities.exceptions import (
+    InputError,
+    SAMExecutionError,
+    SAMInputWarning,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractSamGeneration(RevPySam, ScheduledLossesMixin, ABC):
     """Base class for SAM generation simulations."""
 
-    def __init__(self, resource, meta, sam_sys_inputs, site_sys_inputs=None,
-                 output_request=None, drop_leap=False):
+    def __init__(
+        self,
+        resource,
+        meta,
+        sam_sys_inputs,
+        site_sys_inputs=None,
+        output_request=None,
+        drop_leap=False,
+    ):
         """Initialize a SAM generation object.
 
         Parameters
         ----------
         resource : pd.DataFrame
             Timeseries solar or wind resource data for a single location with a
             pandas DatetimeIndex.  There must be columns for all the required
@@ -84,19 +97,23 @@
             resource = self.drop_leap(resource)
 
         # make sure timezone and elevation are in the meta data
         meta = self.tz_elev_check(sam_sys_inputs, site_sys_inputs, meta)
 
         # don't pass resource to base class,
         # set in concrete generation classes instead
-        super().__init__(meta, sam_sys_inputs, output_request,
-                         site_sys_inputs=site_sys_inputs)
+        super().__init__(
+            meta,
+            sam_sys_inputs,
+            output_request,
+            site_sys_inputs=site_sys_inputs,
+        )
 
         # Set the site number using resource
-        if hasattr(resource, 'name'):
+        if hasattr(resource, "name"):
             self._site = resource.name
         else:
             self._site = None
 
         # let children pass in None resource
         if resource is not None:
             self.check_resource_data(resource)
@@ -160,27 +177,32 @@
         out_req_nomeans : list
             Output request list with the resource mean entries removed.
         """
 
         out_req_nomeans = copy.deepcopy(output_request)
         res_mean = None
         idx = resource.sites.index(res_gid)
-        irrad_means = ('dni_mean', 'dhi_mean', 'ghi_mean',
-                       'clearsky_dni_mean', 'clearsky_dhi_mean',
-                       'clearsky_ghi_mean')
+        irrad_means = (
+            "dni_mean",
+            "dhi_mean",
+            "ghi_mean",
+            "clearsky_dni_mean",
+            "clearsky_dhi_mean",
+            "clearsky_ghi_mean",
+        )
 
-        if 'ws_mean' in out_req_nomeans:
-            out_req_nomeans.remove('ws_mean')
+        if "ws_mean" in out_req_nomeans:
+            out_req_nomeans.remove("ws_mean")
             res_mean = {}
-            res_mean['ws_mean'] = resource['mean_windspeed', idx]
+            res_mean["ws_mean"] = resource["mean_windspeed", idx]
 
         else:
             for var in resource.var_list:
-                label_1 = '{}_mean'.format(var)
-                label_2 = 'mean_{}'.format(var)
+                label_1 = "{}_mean".format(var)
+                label_2 = "mean_{}".format(var)
                 if label_1 in out_req_nomeans:
                     out_req_nomeans.remove(label_1)
                     if res_mean is None:
                         res_mean = {}
                     res_mean[label_1] = resource[label_2, idx]
 
                     if label_1 in irrad_means:
@@ -201,16 +223,17 @@
             variables to run the respective SAM simulation. Remapping will be
             done to convert typical NSRDB/WTK names into SAM names (e.g. DNI ->
             dn and wind_speed -> windspeed)
         """
         if pd.isna(resource).any().any():
             bad_vars = pd.isna(resource).any(axis=0)
             bad_vars = resource.columns[bad_vars].values.tolist()
-            msg = ('Found NaN values for site {} in variables {}'
-                   .format(self.site, bad_vars))
+            msg = "Found NaN values for site {} in variables {}".format(
+                self.site, bad_vars
+            )
             logger.error(msg)
             raise InputError(msg)
 
     @abstractmethod
     def set_resource_data(self, resource, meta):
         """Placeholder for resource data setting (nsrdb or wtk)"""
 
@@ -230,158 +253,184 @@
             Meta data corresponding to the resource input for the single
             location. Should include values for latitude, longitude, elevation,
             and timezone.
 
         Returns
         -------
         meta : pd.DataFrame | pd.Series
-            Datafram or series for a single site. Will include "timezone"
+            Dataframe or series for a single site. Will include "timezone"
             and "elevation" from the sam and site system inputs if found.
         """
 
         if meta is not None:
+            axis = 0 if isinstance(meta, pd.core.series.Series) else 1
+            meta = meta.rename(
+                SupplyCurveField.map_to(ResourceMetaField), axis=axis
+            )
             if sam_sys_inputs is not None:
-                if 'elevation' in sam_sys_inputs:
-                    meta['elevation'] = sam_sys_inputs['elevation']
-                if 'timezone' in sam_sys_inputs:
-                    meta['timezone'] = int(sam_sys_inputs['timezone'])
+                if ResourceMetaField.ELEVATION in sam_sys_inputs:
+                    meta[ResourceMetaField.ELEVATION] = sam_sys_inputs[
+                        ResourceMetaField.ELEVATION
+                    ]
+                if ResourceMetaField.TIMEZONE in sam_sys_inputs:
+                    meta[ResourceMetaField.TIMEZONE] = int(
+                        sam_sys_inputs[ResourceMetaField.TIMEZONE]
+                    )
 
             # site-specific inputs take priority over generic system inputs
             if site_sys_inputs is not None:
-                if 'elevation' in site_sys_inputs:
-                    meta['elevation'] = site_sys_inputs['elevation']
-                if 'timezone' in site_sys_inputs:
-                    meta['timezone'] = int(site_sys_inputs['timezone'])
-
-            if 'timezone' not in meta:
-                msg = ('Need timezone input to run SAM gen. Not found in '
-                       'resource meta or technology json input config.')
+                if ResourceMetaField.ELEVATION in site_sys_inputs:
+                    meta[ResourceMetaField.ELEVATION] = site_sys_inputs[
+                        ResourceMetaField.ELEVATION
+                    ]
+                if ResourceMetaField.TIMEZONE in site_sys_inputs:
+                    meta[ResourceMetaField.TIMEZONE] = int(
+                        site_sys_inputs[ResourceMetaField.TIMEZONE]
+                    )
+
+            if ResourceMetaField.TIMEZONE not in meta:
+                msg = (
+                    "Need timezone input to run SAM gen. Not found in "
+                    "resource meta or technology json input config."
+                )
                 raise SAMExecutionError(msg)
 
         return meta
 
     @property
     def has_timezone(self):
-        """ Returns true if instance has a timezone set """
-        if self._meta is not None:
-            if 'timezone' in self.meta:
-                return True
+        """Returns true if instance has a timezone set"""
+        if self._meta is not None and ResourceMetaField.TIMEZONE in self.meta:
+            return True
 
         return False
 
     def cf_mean(self):
         """Get mean capacity factor (fractional) from SAM.
 
         Returns
         -------
         output : float
             Mean capacity factor (fractional).
         """
-        return self['capacity_factor'] / 100
+        return self["capacity_factor"] / 100
 
     def cf_profile(self):
         """Get hourly capacity factor (frac) profile in local timezone.
         See self.outputs attribute for collected output data in UTC.
 
         Returns
         -------
         cf_profile : np.ndarray
             1D numpy array of capacity factor profile.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return self.gen_profile() / self.sam_sys_inputs['system_capacity']
+        return self.gen_profile() / self.sam_sys_inputs["system_capacity"]
 
     def annual_energy(self):
         """Get annual energy generation value in kWh from SAM.
 
         Returns
         -------
         output : float
             Annual energy generation (kWh).
         """
-        return self['annual_energy']
+        return self["annual_energy"]
 
     def energy_yield(self):
         """Get annual energy yield value in kwh/kw from SAM.
 
         Returns
         -------
         output : float
             Annual energy yield (kwh/kw).
         """
-        return self['kwh_per_kw']
+        return self["kwh_per_kw"]
 
     def gen_profile(self):
         """Get power generation profile (local timezone) in kW.
         See self.outputs attribute for collected output data in UTC.
 
         Returns
         -------
         output : np.ndarray
             1D array of hourly power generation in kW.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return np.array(self['gen'], dtype=np.float32)
+        return np.array(self["gen"], dtype=np.float32)
 
     def collect_outputs(self, output_lookup=None):
         """Collect SAM output_request, convert timeseries outputs to UTC, and
         save outputs to self.outputs property.
 
 
         Parameters
         ----------
         output_lookup : dict | None
             Lookup dictionary mapping output keys to special output methods.
             None defaults to generation default outputs.
         """
 
         if output_lookup is None:
-            output_lookup = {'cf_mean': self.cf_mean,
-                             'cf_profile': self.cf_profile,
-                             'annual_energy': self.annual_energy,
-                             'energy_yield': self.energy_yield,
-                             'gen_profile': self.gen_profile,
-                             }
+            output_lookup = {
+                "cf_mean": self.cf_mean,
+                "cf_profile": self.cf_profile,
+                "annual_energy": self.annual_energy,
+                "energy_yield": self.energy_yield,
+                "gen_profile": self.gen_profile,
+            }
 
         super().collect_outputs(output_lookup=output_lookup)
 
     def run_gen_and_econ(self):
         """Run SAM generation with possibility for follow on econ analysis."""
 
         lcoe_out_reqs = None
         so_out_reqs = None
-        lcoe_vars = ('lcoe_fcr', 'fixed_charge_rate', 'capital_cost',
-                     'fixed_operating_cost', 'variable_operating_cost')
-        so_vars = ('ppa_price', 'lcoe_real', 'lcoe_nom',
-                   'project_return_aftertax_npv', 'flip_actual_irr',
-                   'gross_revenue')
-        if 'lcoe_fcr' in self.output_request:
+        lcoe_vars = (
+            "lcoe_fcr",
+            "fixed_charge_rate",
+            "capital_cost",
+            "fixed_operating_cost",
+            "variable_operating_cost",
+        )
+        so_vars = (
+            "ppa_price",
+            "lcoe_real",
+            "lcoe_nom",
+            "project_return_aftertax_npv",
+            "flip_actual_irr",
+            "gross_revenue",
+        )
+        if "lcoe_fcr" in self.output_request:
             lcoe_out_reqs = [r for r in self.output_request if r in lcoe_vars]
-            self.output_request = [r for r in self.output_request
-                                   if r not in lcoe_out_reqs]
+            self.output_request = [
+                r for r in self.output_request if r not in lcoe_out_reqs
+            ]
         elif any(x in self.output_request for x in so_vars):
             so_out_reqs = [r for r in self.output_request if r in so_vars]
-            self.output_request = [r for r in self.output_request
-                                   if r not in so_out_reqs]
+            self.output_request = [
+                r for r in self.output_request if r not in so_out_reqs
+            ]
 
         # Execute the SAM generation compute module (pvwattsv7, windpower, etc)
         self.run()
 
         # Execute a follow-on SAM econ compute module
         # (lcoe_fcr, singleowner, etc)
         if lcoe_out_reqs is not None:
-            self.sam_sys_inputs['annual_energy'] = self.annual_energy()
+            self.sam_sys_inputs["annual_energy"] = self.annual_energy()
             lcoe = LCOE(self.sam_sys_inputs, output_request=lcoe_out_reqs)
             lcoe.assign_inputs()
             lcoe.execute()
             lcoe.collect_outputs()
             self.outputs.update(lcoe.outputs)
 
         elif so_out_reqs is not None:
-            self.sam_sys_inputs['gen'] = self.gen_profile()
+            self.sam_sys_inputs["gen"] = self.gen_profile()
             so = SingleOwner(self.sam_sys_inputs, output_request=so_out_reqs)
             so.assign_inputs()
             so.execute()
             so.collect_outputs()
             self.outputs.update(so.outputs)
 
     def run(self):
@@ -389,18 +438,26 @@
         SAM simulation, collecting outputs, and converting all arrays to UTC.
         """
         self.assign_inputs()
         self.execute()
         self.collect_outputs()
 
     @classmethod
-    def reV_run(cls, points_control, res_file, site_df,
-                lr_res_file=None, output_request=('cf_mean',),
-                drop_leap=False, gid_map=None, nn_map=None,
-                bias_correct=None):
+    def reV_run(
+        cls,
+        points_control,
+        res_file,
+        site_df,
+        lr_res_file=None,
+        output_request=("cf_mean",),
+        drop_leap=False,
+        gid_map=None,
+        nn_map=None,
+        bias_correct=None,
+    ):
         """Execute SAM generation based on a reV points control instance.
 
         Parameters
         ----------
         points_control : config.PointsControl
             PointsControl instance containing project points site and SAM
             config info.
@@ -456,53 +513,61 @@
             the second level key is the variable name, second level value is
             the output variable value.
         """
         # initialize output dictionary
         out = {}
 
         # Get the RevPySam resource object
-        resources = RevPySam.get_sam_res(res_file,
-                                         points_control.project_points,
-                                         points_control.project_points.tech,
-                                         output_request=output_request,
-                                         gid_map=gid_map,
-                                         lr_res_file=lr_res_file,
-                                         nn_map=nn_map,
-                                         bias_correct=bias_correct)
+        resources = RevPySam.get_sam_res(
+            res_file,
+            points_control.project_points,
+            points_control.project_points.tech,
+            output_request=output_request,
+            gid_map=gid_map,
+            lr_res_file=lr_res_file,
+            nn_map=nn_map,
+            bias_correct=bias_correct,
+        )
 
         # run resource through curtailment filter if applicable
         curtailment = points_control.project_points.curtailment
         if curtailment is not None:
-            resources = curtail(resources, curtailment,
-                                random_seed=curtailment.random_seed)
+            resources = curtail(
+                resources, curtailment, random_seed=curtailment.random_seed
+            )
 
         # iterate through project_points gen_gid values
         for gen_gid in points_control.project_points.sites:
-
             # Lookup the resource gid if there's a mapping and get the resource
             # data from the SAMResource object using the res_gid.
             res_gid = gen_gid if gid_map is None else gid_map[gen_gid]
             site_res_df, site_meta = resources._get_res_df(res_gid)
 
             # drop the leap day
             if drop_leap:
                 site_res_df = cls.drop_leap(site_res_df)
 
             _, inputs = points_control.project_points[gen_gid]
 
             # get resource data pass-throughs and resource means
-            res_outs, out_req_cleaned = cls._get_res(site_res_df,
-                                                     output_request)
-            res_mean, out_req_cleaned = cls._get_res_mean(resources, res_gid,
-                                                          out_req_cleaned)
+            res_outs, out_req_cleaned = cls._get_res(
+                site_res_df, output_request
+            )
+            res_mean, out_req_cleaned = cls._get_res_mean(
+                resources, res_gid, out_req_cleaned
+            )
 
             # iterate through requested sites.
-            sim = cls(resource=site_res_df, meta=site_meta,
-                      sam_sys_inputs=inputs, output_request=out_req_cleaned,
-                      site_sys_inputs=dict(site_df.loc[gen_gid, :]))
+            sim = cls(
+                resource=site_res_df,
+                meta=site_meta,
+                sam_sys_inputs=inputs,
+                output_request=out_req_cleaned,
+                site_sys_inputs=dict(site_df.loc[gen_gid, :]),
+            )
             sim.run_gen_and_econ()
 
             # collect outputs to dictout
             out[gen_gid] = sim.outputs
 
             if res_outs is not None:
                 out[gen_gid].update(res_outs)
@@ -510,18 +575,28 @@
             if res_mean is not None:
                 out[gen_gid].update(res_mean)
 
         return out
 
 
 class AbstractSamGenerationFromWeatherFile(AbstractSamGeneration, ABC):
-    """Base class for running sam generation with a weather file on disk. """
-    WF_META_DROP_COLS = {'elevation', 'timezone', 'country', 'state', 'county',
-                         'urban', 'population', 'landcover', 'latitude',
-                         'longitude'}
+    """Base class for running sam generation with a weather file on disk."""
+
+    WF_META_DROP_COLS = {
+        ResourceMetaField.LATITUDE,
+        ResourceMetaField.LONGITUDE,
+        ResourceMetaField.ELEVATION,
+        ResourceMetaField.TIMEZONE,
+        ResourceMetaField.COUNTRY,
+        ResourceMetaField.STATE,
+        ResourceMetaField.COUNTY,
+        "urban",
+        "population",
+        "landcover",
+    }
 
     @property
     @abstractmethod
     def PYSAM_WEATHER_TAG(self):
         """Name of the weather file input used by SAM generation module."""
         raise NotImplementedError
 
@@ -578,67 +653,70 @@
         -----
         PySAM will not accept data on Feb 29th. For leap years,
         December 31st is dropped and time steps are shifted to relabel
         Feb 29th as March 1st, March 1st as March 2nd, etc.
         """
         # pylint: disable=attribute-defined-outside-init,consider-using-with
         self._temp_dir = TemporaryDirectory()
-        fname = os.path.join(self._temp_dir.name, 'weather.csv')
-        logger.debug('Creating PySAM weather data file: {}'.format(fname))
+        fname = os.path.join(self._temp_dir.name, "weather.csv")
+        logger.debug("Creating PySAM weather data file: {}".format(fname))
 
         # ------- Process metadata
         m = pd.DataFrame(meta).T
-        timezone = m['timezone']
-        m['Source'] = 'NSRDB'
-        m['Location ID'] = meta.name
-        m['City'] = '-'
-        m['State'] = m['state'].apply(lambda x: '-' if x == 'None' else x)
-        m['Country'] = m['country'].apply(lambda x: '-' if x == 'None' else x)
-        m['Latitude'] = m['latitude']
-        m['Longitude'] = m['longitude']
-        m['Time Zone'] = timezone
-        m['Elevation'] = m['elevation']
-        m['Local Time Zone'] = timezone
-        m['Dew Point Units'] = 'c'
-        m['DHI Units'] = 'w/m2'
-        m['DNI Units'] = 'w/m2'
-        m['Temperature Units'] = 'c'
-        m['Pressure Units'] = 'mbar'
-        m['Wind Speed'] = 'm/s'
+        timezone = m[ResourceMetaField.TIMEZONE]
+        m["Source"] = "NSRDB"
+        m["Location ID"] = meta.name
+        m["City"] = "-"
+        m["State"] = m["state"].apply(lambda x: "-" if x == "None" else x)
+        m["Country"] = m["country"].apply(lambda x: "-" if x == "None" else x)
+        m["Latitude"] = m[ResourceMetaField.LATITUDE]
+        m["Longitude"] = m[ResourceMetaField.LONGITUDE]
+        m["Time Zone"] = timezone
+        m["Elevation"] = m[ResourceMetaField.ELEVATION]
+        m["Local Time Zone"] = timezone
+        m["Dew Point Units"] = "c"
+        m["DHI Units"] = "w/m2"
+        m["DNI Units"] = "w/m2"
+        m["Temperature Units"] = "c"
+        m["Pressure Units"] = "mbar"
+        m["Wind Speed"] = "m/s"
         keep_cols = [c for c in m.columns if c not in self.WF_META_DROP_COLS]
-        m[keep_cols].to_csv(fname, index=False, mode='w')
+        m[keep_cols].to_csv(fname, index=False, mode="w")
 
         # --------- Process data
-        var_map = {'dni': 'DNI',
-                   'dhi': 'DHI',
-                   'wind_speed': 'Wind Speed',
-                   'air_temperature': 'Temperature',
-                   'dew_point': 'Dew Point',
-                   'surface_pressure': 'Pressure',
-                   }
-        resource = resource.rename(mapper=var_map, axis='columns')
+        var_map = {
+            "dni": "DNI",
+            "dhi": "DHI",
+            "wind_speed": "Wind Speed",
+            "air_temperature": "Temperature",
+            "dew_point": "Dew Point",
+            "surface_pressure": "Pressure",
+        }
+        resource = resource.rename(mapper=var_map, axis="columns")
 
         time_index = resource.index
         # Adjust from UTC to local time
-        local = np.roll(resource.values, int(timezone * self.time_interval),
-                        axis=0)
-        resource = pd.DataFrame(local, columns=resource.columns,
-                                index=time_index)
+        local = np.roll(
+            resource.values, int(timezone * self.time_interval), axis=0
+        )
+        resource = pd.DataFrame(
+            local, columns=resource.columns, index=time_index
+        )
         mask = (time_index.month == 2) & (time_index.day == 29)
         time_index = time_index[~mask]
 
         df = pd.DataFrame(index=time_index)
-        df['Year'] = time_index.year
-        df['Month'] = time_index.month
-        df['Day'] = time_index.day
-        df['Hour'] = time_index.hour
-        df['Minute'] = time_index.minute
+        df["Year"] = time_index.year
+        df["Month"] = time_index.month
+        df["Day"] = time_index.day
+        df["Hour"] = time_index.hour
+        df["Minute"] = time_index.minute
         df = df.join(resource.loc[~mask])
 
-        df.to_csv(fname, index=False, mode='a')
+        df.to_csv(fname, index=False, mode="a")
 
         return fname
 
     def run_gen_and_econ(self):
         """Run SAM generation and possibility follow-on econ analysis."""
         try:
             super().run_gen_and_econ()
@@ -699,91 +777,104 @@
         """
 
         meta = self._parse_meta(meta)
         time_index = resource.index
         self.time_interval = self.get_time_interval(resource.index.values)
 
         # map resource data names to SAM required data names
-        var_map = {'dni': 'dn',
-                   'dhi': 'df',
-                   'ghi': 'gh',
-                   'clearskydni': 'dn',
-                   'clearskydhi': 'df',
-                   'clearskyghi': 'gh',
-                   'windspeed': 'wspd',
-                   'airtemperature': 'tdry',
-                   'temperature': 'tdry',
-                   'temp': 'tdry',
-                   'dewpoint': 'tdew',
-                   'surfacepressure': 'pres',
-                   'pressure': 'pres',
-                   'surfacealbedo': 'albedo',
-                   }
-        lower_case = {k: k.lower().replace(' ', '').replace('_', '')
-                      for k in resource.columns}
-        irrad_vars = ['dn', 'df', 'gh']
+        var_map = {
+            "dni": "dn",
+            "dhi": "df",
+            "ghi": "gh",
+            "clearskydni": "dn",
+            "clearskydhi": "df",
+            "clearskyghi": "gh",
+            "windspeed": "wspd",
+            "airtemperature": "tdry",
+            "temperature": "tdry",
+            "temp": "tdry",
+            "dewpoint": "tdew",
+            "surfacepressure": "pres",
+            "pressure": "pres",
+            "surfacealbedo": "albedo",
+        }
+        lower_case = {
+            k: k.lower().replace(" ", "").replace("_", "")
+            for k in resource.columns
+        }
+        irrad_vars = ["dn", "df", "gh"]
 
-        resource = resource.rename(mapper=lower_case, axis='columns')
-        resource = resource.rename(mapper=var_map, axis='columns')
+        resource = resource.rename(mapper=lower_case, axis="columns")
+        resource = resource.rename(mapper=var_map, axis="columns")
         time_index = resource.index
-        resource = {k: np.array(v) for (k, v) in
-                    resource.to_dict(orient='list').items()}
+        resource = {
+            k: np.array(v)
+            for (k, v) in resource.to_dict(orient="list").items()
+        }
 
         # set resource variables
         for var, arr in resource.items():
-            if var != 'time_index':
-
+            if var != "time_index":
                 # ensure that resource array length is multiple of 8760
                 arr = self.ensure_res_len(arr, time_index)
-                n_roll = int(self._meta['timezone'] * self.time_interval)
+                n_roll = int(
+                    self._meta[ResourceMetaField.TIMEZONE] * self.time_interval
+                )
                 arr = np.roll(arr, n_roll)
 
-                if var in irrad_vars:
-                    if np.min(arr) < 0:
-                        warn('Solar irradiance variable "{}" has a minimum '
-                             'value of {}. Truncating to zero.'
-                             .format(var, np.min(arr)), SAMInputWarning)
-                        arr = np.where(arr < 0, 0, arr)
+                if var in irrad_vars and np.min(arr) < 0:
+                    warn(
+                        'Solar irradiance variable "{}" has a minimum '
+                        "value of {}. Truncating to zero.".format(
+                            var, np.min(arr)
+                        ),
+                        SAMInputWarning,
+                    )
+                    arr = np.where(arr < 0, 0, arr)
 
                 resource[var] = arr.tolist()
 
-        resource['lat'] = meta['latitude']
-        resource['lon'] = meta['longitude']
-        resource['tz'] = meta['timezone']
+        resource["lat"] = meta[ResourceMetaField.LATITUDE]
+        resource["lon"] = meta[ResourceMetaField.LONGITUDE]
+        resource["tz"] = meta[ResourceMetaField.TIMEZONE]
 
-        if 'elevation' in meta:
-            resource['elev'] = meta['elevation']
-        else:
-            resource['elev'] = 0.0
+        resource["elev"] = meta.get(ResourceMetaField.ELEVATION, 0.0)
 
         time_index = self.ensure_res_len(time_index, time_index)
-        resource['minute'] = time_index.minute
-        resource['hour'] = time_index.hour
-        resource['month'] = time_index.month
-        resource['year'] = time_index.year
-        resource['day'] = time_index.day
-
-        if 'albedo' in resource:
-            self['albedo'] = self.agg_albedo(
-                time_index, resource.pop('albedo'))
+        resource["minute"] = time_index.minute
+        resource["hour"] = time_index.hour
+        resource["month"] = time_index.month
+        resource["year"] = time_index.year
+        resource["day"] = time_index.day
+
+        if "albedo" in resource:
+            self["albedo"] = self.agg_albedo(
+                time_index, resource.pop("albedo")
+            )
 
-        self['solar_resource_data'] = resource
+        self["solar_resource_data"] = resource
 
 
 class AbstractSamPv(AbstractSamSolar, ABC):
-    """Photovoltaic (PV) generation with either pvwatts of detailed pv.
-    """
+    """Photovoltaic (PV) generation with either pvwatts of detailed pv."""
 
     # set these class attrs in concrete subclasses
     MODULE = None
     PYSAM = None
 
     # pylint: disable=line-too-long
-    def __init__(self, resource, meta, sam_sys_inputs, site_sys_inputs=None,
-                 output_request=None, drop_leap=False):
+    def __init__(
+        self,
+        resource,
+        meta,
+        sam_sys_inputs,
+        site_sys_inputs=None,
+        output_request=None,
+        drop_leap=False,
+    ):
         """Initialize a SAM solar object.
 
         See the PySAM :py:class:`~PySAM.Pvwattsv8.Pvwattsv8` (or older
         version model) or :py:class:`~PySAM.Pvsamv1.Pvsamv1` documentation for
         the configuration keys required in the `sam_sys_inputs` config for the
         respective models. Some notable keys include the following to enable a
         lifetime simulation (non-exhaustive):
@@ -874,18 +965,22 @@
             31st is dropped from leap years.
         """
 
         # need to check tilt=lat and azimuth for pv systems
         meta = self._parse_meta(meta)
         sam_sys_inputs = self.set_latitude_tilt_az(sam_sys_inputs, meta)
 
-        super().__init__(resource, meta, sam_sys_inputs,
-                         site_sys_inputs=site_sys_inputs,
-                         output_request=output_request,
-                         drop_leap=drop_leap)
+        super().__init__(
+            resource,
+            meta,
+            sam_sys_inputs,
+            site_sys_inputs=site_sys_inputs,
+            output_request=output_request,
+            drop_leap=drop_leap,
+        )
 
     def set_resource_data(self, resource, meta):
         """Set NSRDB resource data arrays.
 
         Parameters
         ----------
         resource : pd.DataFrame
@@ -901,23 +996,27 @@
 
         Raises
         ------
         ValueError : If lat/lon outside of -90 to 90 and -180 to 180,
                      respectively.
 
         """
-        bad_location_input = ((meta['latitude'] < -90)
-                              | (meta['latitude'] > 90)
-                              | (meta['longitude'] < -180)
-                              | (meta['longitude'] > 180))
+        bad_location_input = (
+            (meta[ResourceMetaField.LATITUDE] < -90)
+            | (meta[ResourceMetaField.LATITUDE] > 90)
+            | (meta[ResourceMetaField.LONGITUDE] < -180)
+            | (meta[ResourceMetaField.LONGITUDE] > 180)
+        )
         if bad_location_input.any():
-            raise ValueError("Detected latitude/longitude values outside of "
-                             "the range -90 to 90 and -180 to 180, "
-                             "respectively. Please ensure input resource data"
-                             "locations conform to these ranges. ")
+            raise ValueError(
+                "Detected latitude/longitude values outside of "
+                "the range -90 to 90 and -180 to 180, "
+                "respectively. Please ensure input resource data"
+                "locations conform to these ranges. "
+            )
         return super().set_resource_data(resource, meta)
 
     @staticmethod
     def set_latitude_tilt_az(sam_sys_inputs, meta):
         """Check if tilt is specified as latitude and set tilt=lat, az=180 or 0
 
         Parameters
@@ -930,99 +1029,108 @@
             and timezone.
 
         Returns
         -------
         sam_sys_inputs : dict
             Site-agnostic SAM system model inputs arguments.
             If for a pv simulation the "tilt" parameter was originally not
-            present or set to 'lat' or 'latitude', the tilt will be set to
-            the absolute value of the latitude found in meta and the azimuth
-            will be 180 if lat>0, 0 if lat<0.
+            present or set to 'lat' or MetaKeyName.LATITUDE, the tilt will be
+            set to the absolute value of the latitude found in meta and the
+            azimuth will be 180 if lat>0, 0 if lat<0.
         """
 
         set_tilt = False
         if sam_sys_inputs is not None and meta is not None:
-            if 'tilt' not in sam_sys_inputs:
-                warn('No tilt specified, setting at latitude.',
-                     SAMInputWarning)
+            if "tilt" not in sam_sys_inputs:
+                warn(
+                    "No tilt specified, setting at latitude.", SAMInputWarning
+                )
+                set_tilt = True
+            elif (
+                sam_sys_inputs["tilt"] == "lat"
+                or sam_sys_inputs["tilt"] == ResourceMetaField.LATITUDE
+            ) or (
+                sam_sys_inputs["tilt"] == "lat"
+                or sam_sys_inputs["tilt"] == ResourceMetaField.LATITUDE
+            ):
                 set_tilt = True
-            else:
-                if (sam_sys_inputs['tilt'] == 'lat'
-                        or sam_sys_inputs['tilt'] == 'latitude'):
-                    set_tilt = True
 
         if set_tilt:
             # set tilt to abs(latitude)
-            sam_sys_inputs['tilt'] = np.abs(meta['latitude'])
-            if meta['latitude'] > 0:
+            sam_sys_inputs["tilt"] = np.abs(meta[ResourceMetaField.LATITUDE])
+            if meta[ResourceMetaField.LATITUDE] > 0:
                 # above the equator, az = 180
-                sam_sys_inputs['azimuth'] = 180
+                sam_sys_inputs["azimuth"] = 180
             else:
                 # below the equator, az = 0
-                sam_sys_inputs['azimuth'] = 0
+                sam_sys_inputs["azimuth"] = 0
 
-            logger.debug('Tilt specified at "latitude", setting tilt to: {}, '
-                         'azimuth to: {}'
-                         .format(sam_sys_inputs['tilt'],
-                                 sam_sys_inputs['azimuth']))
+            logger.debug(
+                'Tilt specified at "latitude", setting tilt to: {}, '
+                "azimuth to: {}".format(
+                    sam_sys_inputs["tilt"], sam_sys_inputs["azimuth"]
+                )
+            )
         return sam_sys_inputs
 
     def system_capacity_ac(self):
         """Get AC system capacity from SAM inputs.
 
         NOTE: AC nameplate = DC nameplate / ILR
 
         Returns
         -------
         cf_profile : float
             AC nameplate = DC nameplate / ILR
         """
-        return (self.sam_sys_inputs['system_capacity']
-                / self.sam_sys_inputs['dc_ac_ratio'])
+        return (
+            self.sam_sys_inputs["system_capacity"]
+            / self.sam_sys_inputs["dc_ac_ratio"]
+        )
 
     def cf_mean(self):
         """Get mean capacity factor (fractional) from SAM.
 
         NOTE: PV capacity factor is the AC power production / the DC nameplate
 
         Returns
         -------
         output : float
             Mean capacity factor (fractional).
             PV CF is calculated as AC power / DC nameplate.
         """
-        return self['capacity_factor'] / 100
+        return self["capacity_factor"] / 100
 
     def cf_mean_ac(self):
         """Get mean AC capacity factor (fractional) from SAM.
 
         NOTE: This value only available in PVWattsV8 and up.
 
         Returns
         -------
         output : float
             Mean AC capacity factor (fractional).
             PV AC CF is calculated as AC power / AC nameplate.
         """
-        return self['capacity_factor_ac'] / 100
+        return self["capacity_factor_ac"] / 100
 
     def cf_profile(self):
         """Get hourly capacity factor (frac) profile in local timezone.
         See self.outputs attribute for collected output data in UTC.
 
         NOTE: PV capacity factor is the AC power production / the DC nameplate
 
         Returns
         -------
         cf_profile : np.ndarray
             1D numpy array of capacity factor profile.
             Datatype is float32 and array length is 8760*time_interval.
             PV CF is calculated as AC power / DC nameplate.
         """
-        return self.gen_profile() / self.sam_sys_inputs['system_capacity']
+        return self.gen_profile() / self.sam_sys_inputs["system_capacity"]
 
     def cf_profile_ac(self):
         """Get hourly AC capacity factor (frac) profile in local timezone.
         See self.outputs attribute for collected output data in UTC.
 
         NOTE: PV AC capacity factor is the AC power production / the AC
         nameplate. AC nameplate = DC nameplate / ILR
@@ -1043,40 +1151,40 @@
 
         Returns
         -------
         output : np.ndarray
             1D array of AC inverter power generation in kW.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return np.array(self['gen'], dtype=np.float32)
+        return np.array(self["gen"], dtype=np.float32)
 
     def ac(self):
         """Get AC inverter power generation profile (local timezone) in kW.
         See self.outputs attribute for collected output data in UTC.
 
         Returns
         -------
         output : np.ndarray
             1D array of AC inverter power generation in kW.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return np.array(self['ac'], dtype=np.float32) / 1000
+        return np.array(self["ac"], dtype=np.float32) / 1000
 
     def dc(self):
         """
         Get DC array power generation profile (local timezone) in kW.
         See self.outputs attribute for collected output data in UTC.
 
         Returns
         -------
         output : np.ndarray
             1D array of DC array power generation in kW.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return np.array(self['dc'], dtype=np.float32) / 1000
+        return np.array(self["dc"], dtype=np.float32) / 1000
 
     def clipped_power(self):
         """
         Get the clipped DC power generated behind the inverter
         (local timezone) in kW.
         See self.outputs attribute for collected output data in UTC.
 
@@ -1104,68 +1212,69 @@
         ----------
         output_lookup : dict | None
             Lookup dictionary mapping output keys to special output methods.
             None defaults to generation default outputs.
         """
 
         if output_lookup is None:
-            output_lookup = {'cf_mean': self.cf_mean,
-                             'cf_mean_ac': self.cf_mean_ac,
-                             'cf_profile': self.cf_profile,
-                             'cf_profile_ac': self.cf_profile_ac,
-                             'annual_energy': self.annual_energy,
-                             'energy_yield': self.energy_yield,
-                             'gen_profile': self.gen_profile,
-                             'ac': self.ac,
-                             'dc': self.dc,
-                             'clipped_power': self.clipped_power,
-                             'system_capacity_ac': self.system_capacity_ac,
-                             }
+            output_lookup = {
+                "cf_mean": self.cf_mean,
+                "cf_mean_ac": self.cf_mean_ac,
+                "cf_profile": self.cf_profile,
+                "cf_profile_ac": self.cf_profile_ac,
+                "annual_energy": self.annual_energy,
+                "energy_yield": self.energy_yield,
+                "gen_profile": self.gen_profile,
+                "ac": self.ac,
+                "dc": self.dc,
+                "clipped_power": self.clipped_power,
+                "system_capacity_ac": self.system_capacity_ac,
+            }
 
         super().collect_outputs(output_lookup=output_lookup)
 
 
 class PvWattsv5(AbstractSamPv):
-    """Photovoltaic (PV) generation with pvwattsv5.
-    """
-    MODULE = 'pvwattsv5'
+    """Photovoltaic (PV) generation with pvwattsv5."""
+
+    MODULE = "pvwattsv5"
     PYSAM = PySamPv5
 
     @staticmethod
     def default():
         """Get the executed default pysam PVWATTSV5 object.
 
         Returns
         -------
         PySAM.Pvwattsv5
         """
         return DefaultPvWattsv5.default()
 
 
 class PvWattsv7(AbstractSamPv):
-    """Photovoltaic (PV) generation with pvwattsv7.
-    """
-    MODULE = 'pvwattsv7'
+    """Photovoltaic (PV) generation with pvwattsv7."""
+
+    MODULE = "pvwattsv7"
     PYSAM = PySamPv7
 
     @staticmethod
     def default():
         """Get the executed default pysam PVWATTSV7 object.
 
         Returns
         -------
         PySAM.Pvwattsv7
         """
         raise NotImplementedError("Pvwattsv7 default file no longer exists!")
 
 
 class PvWattsv8(AbstractSamPv):
-    """Photovoltaic (PV) generation with pvwattsv8.
-    """
-    MODULE = 'pvwattsv8'
+    """Photovoltaic (PV) generation with pvwattsv8."""
+
+    MODULE = "pvwattsv8"
     PYSAM = PySamPv8
 
     @staticmethod
     def default():
         """Get the executed default pysam PVWATTSV8 object.
 
         Returns
@@ -1174,71 +1283,71 @@
         """
         return DefaultPvWattsv8.default()
 
 
 class PvSamv1(AbstractSamPv):
     """Detailed PV model"""
 
-    MODULE = 'Pvsamv1'
+    MODULE = "Pvsamv1"
     PYSAM = PySamDetailedPv
 
     def ac(self):
         """Get AC inverter power generation profile (local timezone) in kW.
         See self.outputs attribute for collected output data in UTC.
 
         Returns
         -------
         output : np.ndarray
             1D array of AC inverter power generation in kW.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return np.array(self['gen'], dtype=np.float32)
+        return np.array(self["gen"], dtype=np.float32)
 
     def dc(self):
         """
         Get DC array power generation profile (local timezone) in kW.
         See self.outputs attribute for collected output data in UTC.
 
         Returns
         -------
         output : np.ndarray
             1D array of DC array power generation in kW.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return np.array(self['dc_net'], dtype=np.float32)
+        return np.array(self["dc_net"], dtype=np.float32)
 
     @staticmethod
     def default():
         """Get the executed default pysam Pvsamv1 object.
 
         Returns
         -------
         PySAM.Pvsamv1
         """
         return DefaultPvSamv1.default()
 
 
 class TcsMoltenSalt(AbstractSamSolar):
-    """Concentrated Solar Power (CSP) generation with tower molten salt
-    """
-    MODULE = 'tcsmolten_salt'
+    """Concentrated Solar Power (CSP) generation with tower molten salt"""
+
+    MODULE = "tcsmolten_salt"
     PYSAM = PySamCSP
 
     def cf_profile(self):
         """Get absolute value hourly capacity factor (frac) profile in
         local timezone.
         See self.outputs attribute for collected output data in UTC.
 
         Returns
         -------
         cf_profile : np.ndarray
             1D numpy array of capacity factor profile.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        x = np.abs(self.gen_profile() / self.sam_sys_inputs['system_capacity'])
+        x = np.abs(self.gen_profile() / self.sam_sys_inputs["system_capacity"])
         return x
 
     @staticmethod
     def default():
         """Get the executed default pysam CSP object.
 
         Returns
@@ -1248,17 +1357,18 @@
         return DefaultTcsMoltenSalt.default()
 
 
 class SolarWaterHeat(AbstractSamGenerationFromWeatherFile):
     """
     Solar Water Heater generation
     """
-    MODULE = 'solarwaterheat'
+
+    MODULE = "solarwaterheat"
     PYSAM = PySamSwh
-    PYSAM_WEATHER_TAG = 'solar_resource_file'
+    PYSAM_WEATHER_TAG = "solar_resource_file"
 
     @staticmethod
     def default():
         """Get the executed default pysam swh object.
 
         Returns
         -------
@@ -1267,30 +1377,32 @@
         return DefaultSwh.default()
 
 
 class LinearDirectSteam(AbstractSamGenerationFromWeatherFile):
     """
     Process heat linear Fresnel direct steam generation
     """
-    MODULE = 'lineardirectsteam'
+
+    MODULE = "lineardirectsteam"
     PYSAM = PySamLds
-    PYSAM_WEATHER_TAG = 'file_name'
+    PYSAM_WEATHER_TAG = "file_name"
 
     def cf_mean(self):
         """Calculate mean capacity factor (fractional) from SAM.
 
         Returns
         -------
         output : float
             Mean capacity factor (fractional).
         """
-        net_power = self['annual_field_energy'] \
-            - self['annual_thermal_consumption']  # kW-hr
+        net_power = (
+            self["annual_field_energy"] - self["annual_thermal_consumption"]
+        )  # kW-hr
         # q_pb_des is in MW, convert to kW-hr
-        name_plate = self['q_pb_des'] * 8760 * 1000
+        name_plate = self["q_pb_des"] * 8760 * 1000
 
         return net_power / name_plate
 
     @staticmethod
     def default():
         """Get the executed default pysam linear Fresnel object.
 
@@ -1301,30 +1413,32 @@
         return DefaultLinearFresnelDsgIph.default()
 
 
 class TroughPhysicalHeat(AbstractSamGenerationFromWeatherFile):
     """
     Trough Physical Process Heat generation
     """
-    MODULE = 'troughphysicalheat'
+
+    MODULE = "troughphysicalheat"
     PYSAM = PySamTpph
-    PYSAM_WEATHER_TAG = 'file_name'
+    PYSAM_WEATHER_TAG = "file_name"
 
     def cf_mean(self):
         """Calculate mean capacity factor (fractional) from SAM.
 
         Returns
         -------
         output : float
             Mean capacity factor (fractional).
         """
-        net_power = self['annual_gross_energy'] \
-            - self['annual_thermal_consumption']  # kW-hr
+        net_power = (
+            self["annual_gross_energy"] - self["annual_thermal_consumption"]
+        )  # kW-hr
         # q_pb_des is in MW, convert to kW-hr
-        name_plate = self['q_pb_design'] * 8760 * 1000
+        name_plate = self["q_pb_design"] * 8760 * 1000
 
         return net_power / name_plate
 
     @staticmethod
     def default():
         """Get the executed default pysam trough object.
 
@@ -1504,19 +1618,20 @@
           used to sample the ``time_index`` in the resource data.
           This can be used to reduce temporal resolution (i.e. for
           30 minute NSRDB input data, ``time_index_step=1`` yields
           the full 30 minute time series as output, while
           ``time_index_step=2`` yields hourly output, and so forth).
 
     """
+
     # Per Matt Prilliman on 2/22/24, it's unclear where this ratio originates,
     # but SAM errors out if it's exceeded.
     MAX_RT_TO_EGS_RATIO = 1.134324
     """Max value of ``resource_temperature``/``EGS_plan_design_temperature``"""
-    MODULE = 'geothermal'
+    MODULE = "geothermal"
     PYSAM = PySamGeothermal
     PYSAM_WEATHER_TAG = "file_name"
     _RESOURCE_POTENTIAL_MULT = 1.001
     _DEFAULT_NUM_CONFIRMATION_WELLS = 2  # SAM GUI default as of 5/26/23
 
     @staticmethod
     def default():
@@ -1534,22 +1649,24 @@
 
         Returns
         -------
         cf_profile : np.ndarray
             1D numpy array of capacity factor profile.
             Datatype is float32 and array length is 8760*time_interval.
         """
-        return self.gen_profile() / self.sam_sys_inputs['nameplate']
+        return self.gen_profile() / self.sam_sys_inputs["nameplate"]
 
     def assign_inputs(self):
         """Assign the self.sam_sys_inputs attribute to the PySAM object."""
         if self.sam_sys_inputs.get("ui_calculations_only"):
-            msg = ('reV requires model run - cannot set '
-                   '"ui_calculations_only" to `True` (1). Automatically '
-                   'setting to `False` (0)!')
+            msg = (
+                "reV requires model run - cannot set "
+                '"ui_calculations_only" to `True` (1). Automatically '
+                "setting to `False` (0)!"
+            )
             logger.warning(msg)
             warn(msg)
             self.sam_sys_inputs["ui_calculations_only"] = 0
         super().assign_inputs()
 
     def set_resource_data(self, resource, meta):
         """Generate the weather file and set the path as an input.
@@ -1576,87 +1693,111 @@
         self._set_resource_temperature(resource)
         self._set_egs_plant_design_temperature()
         self._set_nameplate_to_match_resource_potential(resource)
         self._set_resource_potential_to_match_gross_output()
         self._set_costs()
 
     def _set_resource_temperature(self, resource):
-        """Set resource temp from data if user did not specify it. """
+        """Set resource temp from data if user did not specify it."""
 
         if "resource_temp" in self.sam_sys_inputs:
-            logger.debug("Found 'resource_temp' value in SAM config: {:.2f}"
-                         .format(self.sam_sys_inputs["resource_temp"]))
+            logger.debug(
+                "Found 'resource_temp' value in SAM config: {:.2f}".format(
+                    self.sam_sys_inputs["resource_temp"]
+                )
+            )
             return
 
         val = set(resource["temperature"].unique())
-        logger.debug("Found {} value(s) for 'temperature' in resource data"
-                     .format(len(val)))
+        logger.debug(
+            "Found {} value(s) for 'temperature' in resource data".format(
+                len(val)
+            )
+        )
         if len(val) > 1:
-            msg = ("Found multiple values for 'temperature' for site {}: {}"
-                   .format(self.site, val))
+            msg = (
+                "Found multiple values for 'temperature' for site "
+                "{}: {}".format(self.site, val)
+            )
             logger.error(msg)
             raise InputError(msg)
 
         val = val.pop()
-        logger.debug("Input 'resource_temp' not found in SAM config - setting "
-                     "to {:.2f} based on input resource data."
-                     .format(val))
+        logger.debug(
+            "Input 'resource_temp' not found in SAM config - setting "
+            "to {:.2f} based on input resource data.".format(val)
+        )
         self.sam_sys_inputs["resource_temp"] = val
 
     def _set_egs_plant_design_temperature(self):
         """Set the EGS plant temp to match resource, if necessary"""
         if self.sam_sys_inputs.get("resource_type") != 1:
             return  # Not EGS run
 
         set_egs_pdt_to_rt = self.sam_sys_inputs.get("set_EGS_PDT_to_RT", False)
         egs_plant_design_temp = self.sam_sys_inputs.get("design_temp", 0)
         resource_temp = self.sam_sys_inputs["resource_temp"]
 
         if set_egs_pdt_to_rt:
-            msg = ('Setting EGS plant design temperature ({}C) to match '
-                   'resource temperature ({}C)'
-                   .format(egs_plant_design_temp, resource_temp))
+            msg = (
+                "Setting EGS plant design temperature ({}C) to match "
+                "resource temperature ({}C)".format(
+                    egs_plant_design_temp, resource_temp
+                )
+            )
             logger.info(msg)
             self.sam_sys_inputs["design_temp"] = resource_temp
             return
 
         if egs_plant_design_temp > resource_temp:
-            msg = ('EGS plant design temperature ({}C) exceeds resource '
-                   'temperature ({}C). Lowering EGS plant design temperature '
-                   'to match resource temperature'
-                   .format(egs_plant_design_temp, resource_temp))
+            msg = (
+                "EGS plant design temperature ({}C) exceeds resource "
+                "temperature ({}C). Lowering EGS plant design temperature "
+                "to match resource temperature".format(
+                    egs_plant_design_temp, resource_temp
+                )
+            )
             logger.warning(msg)
             warn(msg)
             self.sam_sys_inputs["design_temp"] = resource_temp
             return
 
         if resource_temp / egs_plant_design_temp > self.MAX_RT_TO_EGS_RATIO:
-            msg = ('EGS plant design temperature ({}C) is lower than resource '
-                   'temperature ({}C) by more than a factor of {}. Increasing '
-                   'EGS plant design temperature to match resource temperature'
-                   .format(egs_plant_design_temp, resource_temp,
-                           self.MAX_RT_TO_EGS_RATIO))
+            msg = (
+                "EGS plant design temperature ({}C) is lower than resource "
+                "temperature ({}C) by more than a factor of {}. Increasing "
+                "EGS plant design temperature to match resource "
+                "temperature".format(
+                    egs_plant_design_temp,
+                    resource_temp,
+                    self.MAX_RT_TO_EGS_RATIO,
+                )
+            )
             logger.warning(msg)
             warn(msg)
             self.sam_sys_inputs["design_temp"] = resource_temp
 
     def _set_nameplate_to_match_resource_potential(self, resource):
-        """Set the nameplate capacity to match the resource potential. """
+        """Set the nameplate capacity to match the resource potential."""
 
         if "nameplate" in self.sam_sys_inputs:
-            msg = ('Found "nameplate" input in config! Resource potential '
-                   'from input data will be ignored. Nameplate capacity is {}'
-                   .format(self.sam_sys_inputs["nameplate"]))
+            msg = (
+                'Found "nameplate" input in config! Resource potential '
+                "from input data will be ignored. Nameplate capacity is "
+                "{}".format(self.sam_sys_inputs["nameplate"])
+            )
             logger.info(msg)
             return
 
         val = set(resource["potential_MW"].unique())
         if len(val) > 1:
-            msg = ('Found multiple values for "potential_MW" for site {}: {}'
-                   .format(self.site, val))
+            msg = (
+                'Found multiple values for "potential_MW" for site '
+                "{}: {}".format(self.site, val)
+            )
             logger.error(msg)
             raise InputError(msg)
 
         val = val.pop() * 1000
 
         logger.debug("Setting the nameplate to {}".format(val))
         self.sam_sys_inputs["nameplate"] = val
@@ -1675,71 +1816,90 @@
         try:
             self.execute()
         except SAMExecutionError:
             self["ui_calculations_only"] = 0
             self.sam_sys_inputs["resource_potential"] = -1
             return
 
-        gross_gen = (getattr(self.pysam.Outputs, "gross_output")
-                     * self._RESOURCE_POTENTIAL_MULT)
+        gross_gen = (
+            self.pysam.Outputs.gross_output * self._RESOURCE_POTENTIAL_MULT
+        )
         if "resource_potential" in self.sam_sys_inputs:
-            msg = ('Setting "resource_potential" is not allowed! Updating '
-                   'user input of {} to match the gross generation: {}'
-                   .format(self.sam_sys_inputs["resource_potential"],
-                           gross_gen))
+            msg = (
+                'Setting "resource_potential" is not allowed! Updating '
+                "user input of {} to match the gross generation: {}".format(
+                    self.sam_sys_inputs["resource_potential"], gross_gen
+                )
+            )
             logger.warning(msg)
             warn(msg)
 
-        logger.debug("Setting the resource potential to {} MW"
-                     .format(gross_gen))
+        logger.debug(
+            "Setting the resource potential to {} MW".format(gross_gen)
+        )
         self.sam_sys_inputs["resource_potential"] = gross_gen
 
-        ncw = self.sam_sys_inputs.pop("num_confirmation_wells",
-                                      self._DEFAULT_NUM_CONFIRMATION_WELLS)
+        ncw = self.sam_sys_inputs.pop(
+            "num_confirmation_wells", self._DEFAULT_NUM_CONFIRMATION_WELLS
+        )
         self.sam_sys_inputs["prod_and_inj_wells_to_drill"] = (
-            getattr(self.pysam.Outputs, "num_wells_getem_output")
+            self.pysam.Outputs.num_wells_getem_output
             - ncw
-            + getattr(self.pysam.Outputs, "num_wells_getem_inj"))
+            + self.pysam.Outputs.num_wells_getem_inj
+        )
         self["ui_calculations_only"] = 0
 
     def _set_costs(self):
         """Set the costs based on gross plant generation."""
-        plant_size_kw = (self.sam_sys_inputs["resource_potential"]
-                         / self._RESOURCE_POTENTIAL_MULT) * 1000
+        plant_size_kw = (
+            self.sam_sys_inputs["resource_potential"]
+            / self._RESOURCE_POTENTIAL_MULT
+        ) * 1000
 
         cc_per_kw = self.sam_sys_inputs.pop("capital_cost_per_kw", None)
         if cc_per_kw is not None:
             capital_cost = cc_per_kw * plant_size_kw
-            logger.debug("Setting the capital_cost to ${:,.2f}"
-                         .format(capital_cost))
+            logger.debug(
+                "Setting the capital_cost to ${:,.2f}".format(capital_cost)
+            )
             self.sam_sys_inputs["capital_cost"] = capital_cost
 
         dc_per_well = self.sam_sys_inputs.pop("drill_cost_per_well", None)
-        num_wells = self.sam_sys_inputs.pop("prod_and_inj_wells_to_drill",
-                                            None)
+        num_wells = self.sam_sys_inputs.pop(
+            "prod_and_inj_wells_to_drill", None
+        )
         if dc_per_well is not None:
             if num_wells is None:
-                msg = ('Could not determine number of wells to be drilled. '
-                       'No drilling costs added!')
+                msg = (
+                    "Could not determine number of wells to be drilled. "
+                    "No drilling costs added!"
+                )
                 logger.warning(msg)
                 warn(msg)
             else:
                 capital_cost = self.sam_sys_inputs["capital_cost"]
                 drill_cost = dc_per_well * num_wells
-                logger.debug("Setting the drilling cost to ${:,.2f} "
-                             "({:.2f} wells at ${:,.2f} per well)"
-                             .format(drill_cost, num_wells, dc_per_well))
+                logger.debug(
+                    "Setting the drilling cost to ${:,.2f} "
+                    "({:.2f} wells at ${:,.2f} per well)".format(
+                        drill_cost, num_wells, dc_per_well
+                    )
+                )
                 self.sam_sys_inputs["capital_cost"] = capital_cost + drill_cost
 
-        foc_per_kw = self.sam_sys_inputs.pop("fixed_operating_cost_per_kw",
-                                             None)
+        foc_per_kw = self.sam_sys_inputs.pop(
+            "fixed_operating_cost_per_kw", None
+        )
         if foc_per_kw is not None:
             fixed_operating_cost = foc_per_kw * plant_size_kw
-            logger.debug("Setting the fixed_operating_cost to ${:,.2f}"
-                         .format(capital_cost))
+            logger.debug(
+                "Setting the fixed_operating_cost to ${:,.2f}".format(
+                    capital_cost
+                )
+            )
             self.sam_sys_inputs["fixed_operating_cost"] = fixed_operating_cost
 
     def _create_pysam_wfile(self, resource, meta):
         """Create PySAM weather input file.
 
         Geothermal module requires a weather file, but does not actually
         require any weather data to run. Therefore, an empty file is
@@ -1765,47 +1925,57 @@
         -----
         PySAM will not accept data on Feb 29th. For leap years,
         December 31st is dropped and time steps are shifted to relabel
         Feb 29th as March 1st, March 1st as March 2nd, etc.
         """
         # pylint: disable=attribute-defined-outside-init, consider-using-with
         self._temp_dir = TemporaryDirectory()
-        fname = os.path.join(self._temp_dir.name, 'weather.csv')
-        logger.debug('Creating PySAM weather data file: {}'.format(fname))
+        fname = os.path.join(self._temp_dir.name, "weather.csv")
+        logger.debug("Creating PySAM weather data file: {}".format(fname))
 
         # ------- Process metadata
         m = pd.DataFrame(meta).T
-        m = m.rename({"latitude": "Latitude", "longitude": "Longitude",
-                      "timezone": "Time Zone"}, axis=1)
-
-        m[["Latitude", "Longitude", "Time Zone"]].to_csv(fname, index=False,
-                                                         mode='w')
+        m = m.rename(
+            {
+                "latitude": "Latitude",
+                "longitude": "Longitude",
+                "timezone": "Time Zone",
+            },
+            axis=1,
+        )
+
+        m[["Latitude", "Longitude", "Time Zone"]].to_csv(
+            fname, index=False, mode="w"
+        )
 
         # --------- Process data, blank for geothermal
         time_index = resource.index
         mask = (time_index.month == 2) & (time_index.day == 29)
         time_index = time_index[~mask]
 
         df = pd.DataFrame(index=time_index)
-        df['Year'] = time_index.year
-        df['Month'] = time_index.month
-        df['Day'] = time_index.day
-        df['Hour'] = time_index.hour
-        df['Minute'] = time_index.minute
-        df.to_csv(fname, index=False, mode='a')
+        df["Year"] = time_index.year
+        df["Month"] = time_index.month
+        df["Day"] = time_index.day
+        df["Hour"] = time_index.hour
+        df["Minute"] = time_index.minute
+        df.to_csv(fname, index=False, mode="a")
 
         return fname
 
     def run_gen_and_econ(self):
         """Run SAM generation and possibility follow-on econ analysis."""
         try:
             super().run_gen_and_econ()
         except SAMExecutionError as e:
-            logger.error("Skipping site {}; received sam error: {}"
-                         .format(self._site, str(e)))
+            logger.error(
+                "Skipping site {}; received sam error: {}".format(
+                    self._site, str(e)
+                )
+            )
             self.outputs = {}
 
 
 class AbstractSamWind(AbstractSamGeneration, PowerCurveLossesMixin, ABC):
     """AbstractSamWind"""
 
     # pylint: disable=line-too-long
@@ -1896,17 +2066,17 @@
             31st is dropped from leap years.
         """
         super().__init__(*args, **kwargs)
         self.add_power_curve_losses()
 
 
 class WindPower(AbstractSamWind):
-    """Class for Wind generation from SAM
-    """
-    MODULE = 'windpower'
+    """Class for Wind generation from SAM"""
+
+    MODULE = "windpower"
     PYSAM = PySamWindPower
 
     def set_resource_data(self, resource, meta):
         """Set WTK resource data arrays.
 
         Parameters
         ----------
@@ -1921,68 +2091,71 @@
             location. Should include values for latitude, longitude, elevation,
             and timezone.
         """
 
         meta = self._parse_meta(meta)
 
         # map resource data names to SAM required data names
-        var_map = {'speed': 'windspeed',
-                   'direction': 'winddirection',
-                   'airtemperature': 'temperature',
-                   'temp': 'temperature',
-                   'surfacepressure': 'pressure',
-                   'relativehumidity': 'rh',
-                   'humidity': 'rh',
-                   }
-        lower_case = {k: k.lower().replace(' ', '').replace('_', '')
-                      for k in resource.columns}
-        resource = resource.rename(mapper=lower_case, axis='columns')
-        resource = resource.rename(mapper=var_map, axis='columns')
+        var_map = {
+            "speed": "windspeed",
+            "direction": "winddirection",
+            "airtemperature": "temperature",
+            "temp": "temperature",
+            "surfacepressure": "pressure",
+            "relativehumidity": "rh",
+            "humidity": "rh",
+        }
+        lower_case = {
+            k: k.lower().replace(" ", "").replace("_", "")
+            for k in resource.columns
+        }
+        resource = resource.rename(mapper=lower_case, axis="columns")
+        resource = resource.rename(mapper=var_map, axis="columns")
 
         data_dict = {}
-        var_list = ['temperature', 'pressure', 'windspeed', 'winddirection']
-        if 'winddirection' not in resource:
-            resource['winddirection'] = 0.0
+        var_list = ["temperature", "pressure", "windspeed", "winddirection"]
+        if "winddirection" not in resource:
+            resource["winddirection"] = 0.0
 
         time_index = resource.index
         self.time_interval = self.get_time_interval(resource.index.values)
 
-        data_dict['fields'] = [1, 2, 3, 4]
-        data_dict['heights'] = 4 * [self.sam_sys_inputs['wind_turbine_hub_ht']]
+        data_dict["fields"] = [1, 2, 3, 4]
+        data_dict["heights"] = 4 * [self.sam_sys_inputs["wind_turbine_hub_ht"]]
 
-        if 'rh' in resource:
+        if "rh" in resource:
             # set relative humidity for icing.
-            rh = self.ensure_res_len(resource['rh'].values, time_index)
-            n_roll = int(meta['timezone'] * self.time_interval)
+            rh = self.ensure_res_len(resource["rh"].values, time_index)
+            n_roll = int(meta[ResourceMetaField.TIMEZONE] * self.time_interval)
             rh = np.roll(rh, n_roll, axis=0)
-            data_dict['rh'] = rh.tolist()
+            data_dict["rh"] = rh.tolist()
 
         # must be set as matrix in [temperature, pres, speed, direction] order
         # ensure that resource array length is multiple of 8760
         # roll the truncated resource array to local timezone
         temp = self.ensure_res_len(resource[var_list].values, time_index)
-        n_roll = int(meta['timezone'] * self.time_interval)
+        n_roll = int(meta[ResourceMetaField.TIMEZONE] * self.time_interval)
         temp = np.roll(temp, n_roll, axis=0)
-        data_dict['data'] = temp.tolist()
+        data_dict["data"] = temp.tolist()
 
-        data_dict['lat'] = float(meta['latitude'])
-        data_dict['lon'] = float(meta['longitude'])
-        data_dict['tz'] = int(meta['timezone'])
-        data_dict['elev'] = float(meta['elevation'])
+        data_dict["lat"] = float(meta[ResourceMetaField.LATITUDE])
+        data_dict["lon"] = float(meta[ResourceMetaField.LONGITUDE])
+        data_dict["tz"] = int(meta[ResourceMetaField.TIMEZONE])
+        data_dict["elev"] = float(meta[ResourceMetaField.ELEVATION])
 
         time_index = self.ensure_res_len(time_index, time_index)
-        data_dict['minute'] = time_index.minute.tolist()
-        data_dict['hour'] = time_index.hour.tolist()
-        data_dict['year'] = time_index.year.tolist()
-        data_dict['month'] = time_index.month.tolist()
-        data_dict['day'] = time_index.day.tolist()
+        data_dict["minute"] = time_index.minute.tolist()
+        data_dict["hour"] = time_index.hour.tolist()
+        data_dict["year"] = time_index.year.tolist()
+        data_dict["month"] = time_index.month.tolist()
+        data_dict["day"] = time_index.day.tolist()
 
         # add resource data to self.data and clear
-        self['wind_resource_data'] = data_dict
-        self['wind_resource_model_choice'] = 0
+        self["wind_resource_data"] = data_dict
+        self["wind_resource_model_choice"] = 0
 
     @staticmethod
     def default():
         """Get the executed default pysam WindPower object.
 
         Returns
         -------
@@ -1992,20 +2165,27 @@
 
 
 # pylint: disable=too-many-ancestors
 class WindPowerPD(AbstractSamGeneration, PowerCurveLossesMixin):
     """WindPower analysis with wind speed/direction joint probabilty
     distrubtion input"""
 
-    MODULE = 'windpower'
+    MODULE = "windpower"
     PYSAM = PySamWindPower
 
-    def __init__(self, ws_edges, wd_edges, wind_dist,
-                 meta, sam_sys_inputs,
-                 site_sys_inputs=None, output_request=None):
+    def __init__(
+        self,
+        ws_edges,
+        wd_edges,
+        wind_dist,
+        meta,
+        sam_sys_inputs,
+        site_sys_inputs=None,
+        output_request=None,
+    ):
         """Initialize a SAM generation object for windpower with a
         speed/direction joint probability distribution.
 
         Parameters
         ----------
         ws_edges : np.ndarray
             1D array of windspeed (m/s) values that set the bin edges for the
@@ -2031,21 +2211,25 @@
         """
 
         # make sure timezone and elevation are in the meta data
         meta = self.tz_elev_check(sam_sys_inputs, site_sys_inputs, meta)
 
         # don't pass resource to base class,
         # set in concrete generation classes instead
-        super().__init__(None, meta, sam_sys_inputs,
-                         site_sys_inputs=site_sys_inputs,
-                         output_request=output_request,
-                         drop_leap=False)
+        super().__init__(
+            None,
+            meta,
+            sam_sys_inputs,
+            site_sys_inputs=site_sys_inputs,
+            output_request=output_request,
+            drop_leap=False,
+        )
 
         # Set the site number using meta data
-        if hasattr(meta, 'name'):
+        if hasattr(meta, "name"):
             self._site = meta.name
         else:
             self._site = None
 
         self.set_resource_data(ws_edges, wd_edges, wind_dist)
         self.add_power_curve_losses()
 
@@ -2070,27 +2254,29 @@
         wind_dist /= wind_dist.sum()
 
         # SAM wants the midpoints of the sample bins
         ws_points = ws_edges[:-1] + np.diff(ws_edges) / 2
         wd_points = wd_edges[:-1] + np.diff(wd_edges) / 2
 
         wd_points, ws_points = np.meshgrid(wd_points, ws_points)
-        vstack = (ws_points.flatten(),
-                  wd_points.flatten(),
-                  wind_dist.flatten())
+        vstack = (
+            ws_points.flatten(),
+            wd_points.flatten(),
+            wind_dist.flatten(),
+        )
         wrd = np.vstack(vstack).T.tolist()
 
-        self['wind_resource_model_choice'] = 2
-        self['wind_resource_distribution'] = wrd
+        self["wind_resource_model_choice"] = 2
+        self["wind_resource_distribution"] = wrd
 
 
 class MhkWave(AbstractSamGeneration):
-    """Class for Wave generation from SAM
-    """
-    MODULE = 'mhkwave'
+    """Class for Wave generation from SAM"""
+
+    MODULE = "mhkwave"
     PYSAM = PySamMhkWave
 
     def set_resource_data(self, resource, meta):
         """Set Hindcast US Wave resource data arrays.
 
         Parameters
         ----------
@@ -2103,54 +2289,57 @@
             location. Should include values for latitude, longitude, elevation,
             and timezone.
         """
 
         meta = self._parse_meta(meta)
 
         # map resource data names to SAM required data names
-        var_map = {'significantwaveheight': 'significant_wave_height',
-                   'waveheight': 'significant_wave_height',
-                   'height': 'significant_wave_height',
-                   'swh': 'significant_wave_height',
-                   'energyperiod': 'energy_period',
-                   'waveperiod': 'energy_period',
-                   'period': 'energy_period',
-                   'ep': 'energy_period',
-                   }
-        lower_case = {k: k.lower().replace(' ', '').replace('_', '')
-                      for k in resource.columns}
-        resource = resource.rename(mapper=lower_case, axis='columns')
-        resource = resource.rename(mapper=var_map, axis='columns')
+        var_map = {
+            "significantwaveheight": "significant_wave_height",
+            "waveheight": "significant_wave_height",
+            "height": "significant_wave_height",
+            "swh": "significant_wave_height",
+            "energyperiod": "energy_period",
+            "waveperiod": "energy_period",
+            "period": "energy_period",
+            "ep": "energy_period",
+        }
+        lower_case = {
+            k: k.lower().replace(" ", "").replace("_", "")
+            for k in resource.columns
+        }
+        resource = resource.rename(mapper=lower_case, axis="columns")
+        resource = resource.rename(mapper=var_map, axis="columns")
 
         data_dict = {}
 
         time_index = resource.index
         self.time_interval = self.get_time_interval(resource.index.values)
 
         # must be set as matrix in [temperature, pres, speed, direction] order
         # ensure that resource array length is multiple of 8760
         # roll the truncated resource array to local timezone
-        for var in ['significant_wave_height', 'energy_period']:
+        for var in ["significant_wave_height", "energy_period"]:
             arr = self.ensure_res_len(resource[var].values, time_index)
-            n_roll = int(meta['timezone'] * self.time_interval)
+            n_roll = int(meta[ResourceMetaField.TIMEZONE] * self.time_interval)
             data_dict[var] = np.roll(arr, n_roll, axis=0).tolist()
 
-        data_dict['lat'] = meta['latitude']
-        data_dict['lon'] = meta['longitude']
-        data_dict['tz'] = meta['timezone']
+        data_dict["lat"] = meta[ResourceMetaField.LATITUDE]
+        data_dict["lon"] = meta[ResourceMetaField.LONGITUDE]
+        data_dict["tz"] = meta[ResourceMetaField.TIMEZONE]
 
         time_index = self.ensure_res_len(time_index, time_index)
-        data_dict['minute'] = time_index.minute
-        data_dict['hour'] = time_index.hour
-        data_dict['year'] = time_index.year
-        data_dict['month'] = time_index.month
-        data_dict['day'] = time_index.day
+        data_dict["minute"] = time_index.minute
+        data_dict["hour"] = time_index.hour
+        data_dict["year"] = time_index.year
+        data_dict["month"] = time_index.month
+        data_dict["day"] = time_index.day
 
         # add resource data to self.data and clear
-        self['wave_resource_data'] = data_dict
+        self["wave_resource_data"] = data_dict
 
     @staticmethod
     def default():
         """Get the executed default PySAM MhkWave object.
 
         Returns
         -------
```

### Comparing `NREL-reV-0.8.7/reV/SAM/version_checker.py` & `NREL-reV-0.8.9/reV/SAM/version_checker.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/SAM/windbos.py` & `NREL-reV-0.8.9/reV/SAM/windbos.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,162 +1,168 @@
 # -*- coding: utf-8 -*-
-"""
-SAM Wind Balance of System Cost Model
-"""
+"""SAM Wind Balance of System Cost Model"""
+
 from copy import deepcopy
+
 import numpy as np
 from PySAM.PySSC import ssc_sim_from_dict
 
 from reV.utilities.exceptions import SAMInputError
 
 
 class WindBos:
     """Wind Balance of System Cost Model."""
 
-    MODULE = 'windbos'
+    MODULE = "windbos"
 
     # keys for the windbos input data dictionary.
     # Some keys may not be found explicitly in the SAM input.
-    KEYS = ('tech_model',
-            'financial_model',
-            'machine_rating',
-            'rotor_diameter',
-            'hub_height',
-            'number_of_turbines',
-            'interconnect_voltage',
-            'distance_to_interconnect',
-            'site_terrain',
-            'turbine_layout',
-            'soil_condition',
-            'construction_time',
-            'om_building_size',
-            'quantity_test_met_towers',
-            'quantity_permanent_met_towers',
-            'weather_delay_days',
-            'crane_breakdowns',
-            'access_road_entrances',
-            'turbine_capital_cost',
-            'turbine_cost_per_kw',
-            'tower_top_mass',
-            'delivery_assist_required',
-            'pad_mount_transformer_required',
-            'new_switchyard_required',
-            'rock_trenching_required',
-            'mv_thermal_backfill',
-            'mv_overhead_collector',
-            'performance_bond',
-            'contingency',
-            'warranty_management',
-            'sales_and_use_tax',
-            'overhead',
-            'profit_margin',
-            'development_fee',
-            'turbine_transportation')
+    KEYS = (
+        "tech_model",
+        "financial_model",
+        "machine_rating",
+        "rotor_diameter",
+        "hub_height",
+        "number_of_turbines",
+        "interconnect_voltage",
+        "distance_to_interconnect",
+        "site_terrain",
+        "turbine_layout",
+        "soil_condition",
+        "construction_time",
+        "om_building_size",
+        "quantity_test_met_towers",
+        "quantity_permanent_met_towers",
+        "weather_delay_days",
+        "crane_breakdowns",
+        "access_road_entrances",
+        "turbine_capital_cost",
+        "turbine_cost_per_kw",
+        "tower_top_mass",
+        "delivery_assist_required",
+        "pad_mount_transformer_required",
+        "new_switchyard_required",
+        "rock_trenching_required",
+        "mv_thermal_backfill",
+        "mv_overhead_collector",
+        "performance_bond",
+        "contingency",
+        "warranty_management",
+        "sales_and_use_tax",
+        "overhead",
+        "profit_margin",
+        "development_fee",
+        "turbine_transportation",
+    )
 
     def __init__(self, inputs):
         """
         Parameters
         ----------
         inputs : dict
             SAM key value pair inputs.
         """
 
         self._turbine_capital_cost = 0.0
         self._datadict = {}
 
         self._inputs = inputs
-        self._special = {'tech_model': 'windbos',
-                         'financial_model': 'none',
-                         'machine_rating': self.machine_rating,
-                         'hub_height': self.hub_height,
-                         'rotor_diameter': self.rotor_diameter,
-                         'number_of_turbines': self.number_of_turbines,
-                         'turbine_capital_cost': self.turbine_capital_cost,
-                         }
+        self._special = {
+            "tech_model": "windbos",
+            "financial_model": "none",
+            "machine_rating": self.machine_rating,
+            "hub_height": self.hub_height,
+            "rotor_diameter": self.rotor_diameter,
+            "number_of_turbines": self.number_of_turbines,
+            "turbine_capital_cost": self.turbine_capital_cost,
+        }
         self._parse_inputs()
         self._out = ssc_sim_from_dict(self._datadict)
 
     def _parse_inputs(self):
         """Parse SAM inputs into a windbos input dict and perform any
         required special operations."""
 
         for k in self.KEYS:
             if k in self._special:
                 self._datadict[k] = self._special[k]
             elif k not in self._inputs:
-                raise SAMInputError('Windbos requires input key: "{}"'
-                                    .format(k))
+                raise SAMInputError(
+                    'Windbos requires input key: "{}"'.format(k)
+                )
             else:
                 self._datadict[k] = self._inputs[k]
 
     @property
     def machine_rating(self):
         """Single turbine machine rating either from input or power curve."""
-        if 'machine_rating' in self._inputs:
-            return self._inputs['machine_rating']
+        if "machine_rating" in self._inputs:
+            return self._inputs["machine_rating"]
         else:
-            return np.max(self._inputs['wind_turbine_powercurve_powerout'])
+            return np.max(self._inputs["wind_turbine_powercurve_powerout"])
 
     @property
     def hub_height(self):
         """Turbine hub height."""
-        if 'wind_turbine_hub_ht' in self._inputs:
-            return self._inputs['wind_turbine_hub_ht']
+        if "wind_turbine_hub_ht" in self._inputs:
+            return self._inputs["wind_turbine_hub_ht"]
         else:
-            return self._inputs['hub_height']
+            return self._inputs["hub_height"]
 
     @property
     def rotor_diameter(self):
         """Turbine rotor diameter."""
-        if 'wind_turbine_rotor_diameter' in self._inputs:
-            return self._inputs['wind_turbine_rotor_diameter']
+        if "wind_turbine_rotor_diameter" in self._inputs:
+            return self._inputs["wind_turbine_rotor_diameter"]
         else:
-            return self._inputs['rotor_diameter']
+            return self._inputs["rotor_diameter"]
 
     @property
     def number_of_turbines(self):
         """Number of turbines either based on input or system (farm) capacity
         and machine rating"""
 
-        if 'number_of_turbines' in self._inputs:
-            return self._inputs['number_of_turbines']
+        if "number_of_turbines" in self._inputs:
+            return self._inputs["number_of_turbines"]
         else:
-            return self._inputs['system_capacity'] / self.machine_rating
+            return (
+                self._inputs['system_capacity'] / self.machine_rating
+            )
 
     @property
     def turbine_capital_cost(self):
         """Returns zero (no turbine capital cost for WindBOS input,
         and assigns any input turbine_capital_cost to an attr"""
 
-        if 'turbine_capital_cost' in self._inputs:
-            self._turbine_capital_cost = self._inputs['turbine_capital_cost']
+        if "turbine_capital_cost" in self._inputs:
+            self._turbine_capital_cost = self._inputs["turbine_capital_cost"]
         else:
             self._turbine_capital_cost = 0.0
         return 0.0
 
     @property
     def bos_cost(self):
         """Get the balance of system cost ($)."""
-        return self._out['project_total_budgeted_cost']
+        return self._out["project_total_budgeted_cost"]
 
     @property
     def turbine_cost(self):
         """Get the turbine cost ($)."""
-        tcost = ((self._inputs['turbine_cost_per_kw']
-                  * self.machine_rating
-                  * self.number_of_turbines)
-                 + (self._turbine_capital_cost
-                    * self.number_of_turbines))
+        tcost = (
+            self._inputs["turbine_cost_per_kw"]
+            * self.machine_rating
+            * self.number_of_turbines
+        ) + (self._turbine_capital_cost * self.number_of_turbines)
         return tcost
 
     @property
     def sales_tax_mult(self):
         """Get a sales tax multiplier (frac of the total installed cost)."""
-        basis = self._inputs.get('sales_tax_basis', 0) / 100
-        tax = self._datadict.get('sales_and_use_tax', 0) / 100
+        basis = self._inputs.get("sales_tax_basis", 0) / 100
+        tax = self._datadict.get("sales_and_use_tax", 0) / 100
         return basis * tax
 
     @property
     def sales_tax_cost(self):
         """Get the cost of sales tax ($)."""
         return (self.bos_cost + self.turbine_cost) * self.sales_tax_mult
 
@@ -164,24 +170,31 @@
     def total_installed_cost(self):
         """Get the total installed cost ($) (bos + turbine)."""
         return self.bos_cost + self.turbine_cost + self.sales_tax_cost
 
     @property
     def output(self):
         """Get a dictionary containing the cost breakdown."""
-        output = {'total_installed_cost': self.total_installed_cost,
-                  'turbine_cost': self.turbine_cost,
-                  'sales_tax_cost': self.sales_tax_cost,
-                  'bos_cost': self.bos_cost}
+        output = {
+            "total_installed_cost": self.total_installed_cost,
+            "turbine_cost": self.turbine_cost,
+            "sales_tax_cost": self.sales_tax_cost,
+            "bos_cost": self.bos_cost,
+        }
         return output
 
     # pylint: disable-msg=W0613
     @classmethod
-    def reV_run(cls, points_control, site_df,
-                output_request=('total_installed_cost',), **kwargs):
+    def reV_run(
+        cls,
+        points_control,
+        site_df,
+        output_request=("total_installed_cost",),
+        **kwargs,
+    ):
         """Execute SAM SingleOwner simulations based on reV points control.
 
         Parameters
         ----------
         points_control : config.PointsControl
             PointsControl instance containing project points site and SAM
             config info.
@@ -212,11 +225,12 @@
             # ensure that site-specific data is not persisted to other sites
             site_inputs = deepcopy(inputs)
 
             site_inputs.update(dict(site_df.loc[site, :]))
 
             wb = cls(site_inputs)
 
-            out[site] = {k: v for k, v in wb.output.items()
-                         if k in output_request}
+            out[site] = {
+                k: v for k, v in wb.output.items() if k in output_request
+            }
 
         return out
```

### Comparing `NREL-reV-0.8.7/reV/__init__.py` & `NREL-reV-0.8.9/reV/__init__.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/bespoke/bespoke.py` & `NREL-reV-0.8.9/reV/bespoke/bespoke.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 # -*- coding: utf-8 -*-
 """
 reV bespoke wind plant analysis tools
 """
+
 # pylint: disable=anomalous-backslash-in-string
-from inspect import signature
-import time
-import logging
 import copy
-import pandas as pd
-import numpy as np
-import os
 import json
-import psutil
+import logging
+import os
+import time
+from concurrent.futures import as_completed
 from importlib import import_module
+from inspect import signature
 from numbers import Number
-from concurrent.futures import as_completed
 from warnings import warn
 
+import numpy as np
+import pandas as pd
+import psutil
+from rex.joint_pd.joint_pd import JointPD
+from rex.multi_year_resource import MultiYearWindResource
+from rex.renewable_resource import WindResource
+from rex.utilities.bc_parse_table import parse_bc_table
+from rex.utilities.execution import SpawnProcessPool
+from rex.utilities.loggers import create_dirs, log_mem
+from rex.utilities.utilities import parse_year
+
 from reV.config.output_request import SAMOutputRequest
-from reV.generation.generation import Gen
-from reV.SAM.generation import WindPower, WindPowerPD
 from reV.econ.utilities import lcoe_fcr
-from reV.handlers.outputs import Outputs
+from reV.generation.generation import Gen
 from reV.handlers.exclusions import ExclusionLayers
+from reV.handlers.outputs import Outputs
+from reV.SAM.generation import WindPower, WindPowerPD
+from reV.supply_curve.aggregation import AggFileHandler, BaseAggregation
 from reV.supply_curve.extent import SupplyCurveExtent
 from reV.supply_curve.points import AggregationSupplyCurvePoint as AggSCPoint
 from reV.supply_curve.points import SupplyCurvePoint
-from reV.supply_curve.aggregation import BaseAggregation, AggFileHandler
-from reV.utilities.exceptions import (EmptySupplyCurvePointError,
-                                      FileInputError)
-from reV.utilities import log_versions, ModuleName
-
-from rex.utilities.bc_parse_table import parse_bc_table
-from rex.joint_pd.joint_pd import JointPD
-from rex.renewable_resource import WindResource
-from rex.multi_year_resource import MultiYearWindResource
-from rex.utilities.loggers import log_mem, create_dirs
-from rex.utilities.utilities import parse_year
-from rex.utilities.execution import SpawnProcessPool
+from reV.utilities import (
+    ModuleName,
+    ResourceMetaField,
+    SupplyCurveField,
+    log_versions,
+)
+from reV.utilities.exceptions import EmptySupplyCurvePointError, FileInputError
 
 logger = logging.getLogger(__name__)
 
 
 class BespokeMultiPlantData:
     """Multi-plant preloaded data.
 
@@ -75,42 +80,52 @@
         self._wind_speeds = None
         self._temps = None
         self._pressures = None
         self._time_index = None
         self._pre_load_data()
 
     def _pre_load_data(self):
-        """Pre-load the resource data. """
+        """Pre-load the resource data."""
 
         for sc_gid, gids in self.sc_gid_to_res_gid.items():
             hh = self.sc_gid_to_hh[sc_gid]
             self.hh_to_res_gids.setdefault(hh, set()).update(gids)
 
-        self.hh_to_res_gids = {hh: sorted(gids)
-                               for hh, gids in self.hh_to_res_gids.items()}
+        self.hh_to_res_gids = {
+            hh: sorted(gids) for hh, gids in self.hh_to_res_gids.items()
+        }
 
         start_time = time.time()
-        if '*' in self.res_fpath:
+        if "*" in self.res_fpath:
             handler = MultiYearWindResource
         else:
             handler = WindResource
 
         with handler(self.res_fpath) as res:
-            self._wind_dirs = {hh: res[f"winddirection_{hh}m", :, gids]
-                               for hh, gids in self.hh_to_res_gids.items()}
-            self._wind_speeds = {hh: res[f"windspeed_{hh}m", :, gids]
-                                 for hh, gids in self.hh_to_res_gids.items()}
-            self._temps = {hh: res[f"temperature_{hh}m", :, gids]
-                           for hh, gids in self.hh_to_res_gids.items()}
-            self._pressures = {hh: res[f"pressure_{hh}m", :, gids]
-                               for hh, gids in self.hh_to_res_gids.items()}
+            self._wind_dirs = {
+                hh: res[f"winddirection_{hh}m", :, gids]
+                for hh, gids in self.hh_to_res_gids.items()
+            }
+            self._wind_speeds = {
+                hh: res[f"windspeed_{hh}m", :, gids]
+                for hh, gids in self.hh_to_res_gids.items()
+            }
+            self._temps = {
+                hh: res[f"temperature_{hh}m", :, gids]
+                for hh, gids in self.hh_to_res_gids.items()
+            }
+            self._pressures = {
+                hh: res[f"pressure_{hh}m", :, gids]
+                for hh, gids in self.hh_to_res_gids.items()
+            }
             self._time_index = res.time_index
 
-        logger.debug(f"Data took {(time.time() - start_time) / 60:.2f} "
-                     f"min to load")
+        logger.debug(
+            f"Data took {(time.time() - start_time) / 60:.2f} " f"min to load"
+        )
 
     def get_preloaded_data_for_gid(self, sc_gid):
         """Get the pre-loaded data for a single SC GID.
 
         Parameters
         ----------
         sc_gid : int
@@ -121,32 +136,35 @@
         BespokeSinglePlantData
             A loaded ``BespokeSinglePlantData`` object that can act as
             an HDF5 handler stand-in *for this SC GID only*.
         """
         hh = self.sc_gid_to_hh[sc_gid]
         sc_point_res_gids = sorted(self.sc_gid_to_res_gid[sc_gid])
         data_inds = np.searchsorted(self.hh_to_res_gids[hh], sc_point_res_gids)
-        return BespokeSinglePlantData(sc_point_res_gids,
-                                      self._wind_dirs[hh][:, data_inds],
-                                      self._wind_speeds[hh][:, data_inds],
-                                      self._temps[hh][:, data_inds],
-                                      self._pressures[hh][:, data_inds],
-                                      self._time_index)
+        return BespokeSinglePlantData(
+            sc_point_res_gids,
+            self._wind_dirs[hh][:, data_inds],
+            self._wind_speeds[hh][:, data_inds],
+            self._temps[hh][:, data_inds],
+            self._pressures[hh][:, data_inds],
+            self._time_index,
+        )
 
 
 class BespokeSinglePlantData:
     """Single-plant preloaded data.
 
     This object is intended to facilitate the use of pre-loaded data for
     running :class:`BespokeSinglePlant` on systems with slow parallel
     reads to a single HDF5 file.
     """
 
-    def __init__(self, data_inds, wind_dirs, wind_speeds, temps, pressures,
-                 time_index):
+    def __init__(
+        self, data_inds, wind_dirs, wind_speeds, temps, pressures, time_index
+    ):
         """Initialize BespokeSinglePlantData
 
         Parameters
         ----------
         data_inds : 1D np.array
             Array of res GIDs. This array should be the same length as
             the second dimension of `wind_dirs`, `wind_speeds`, `temps`,
@@ -182,32 +200,51 @@
             return self.pressures[t_idx, data_inds]
         msg = f"Unknown dataset name: {dset_name!r}"
         logger.error(msg)
         raise ValueError(msg)
 
 
 class BespokeSinglePlant:
-    """Framework for analyzing and optimized a wind plant layout specific to
+    """Framework for analyzing and optimizing a wind plant layout specific to
     the local wind resource and exclusions for a single reV supply curve point.
     """
 
-    DEPENDENCIES = ('shapely',)
+    DEPENDENCIES = ("shapely",)
     OUT_ATTRS = copy.deepcopy(Gen.OUT_ATTRS)
 
-    def __init__(self, gid, excl, res, tm_dset, sam_sys_inputs,
-                 objective_function, capital_cost_function,
-                 fixed_operating_cost_function,
-                 variable_operating_cost_function,
-                 min_spacing='5x', wake_loss_multiplier=1, ga_kwargs=None,
-                 output_request=('system_capacity', 'cf_mean'),
-                 ws_bins=(0.0, 20.0, 5.0), wd_bins=(0.0, 360.0, 45.0),
-                 excl_dict=None, inclusion_mask=None, data_layers=None,
-                 resolution=64, excl_area=None, exclusion_shape=None,
-                 eos_mult_baseline_cap_mw=200, prior_meta=None, gid_map=None,
-                 bias_correct=None, pre_loaded_data=None, close=True):
+    def __init__(
+        self,
+        gid,
+        excl,
+        res,
+        tm_dset,
+        sam_sys_inputs,
+        objective_function,
+        capital_cost_function,
+        fixed_operating_cost_function,
+        variable_operating_cost_function,
+        min_spacing="5x",
+        wake_loss_multiplier=1,
+        ga_kwargs=None,
+        output_request=("system_capacity", "cf_mean"),
+        ws_bins=(0.0, 20.0, 5.0),
+        wd_bins=(0.0, 360.0, 45.0),
+        excl_dict=None,
+        inclusion_mask=None,
+        data_layers=None,
+        resolution=64,
+        excl_area=None,
+        exclusion_shape=None,
+        eos_mult_baseline_cap_mw=200,
+        prior_meta=None,
+        gid_map=None,
+        bias_correct=None,
+        pre_loaded_data=None,
+        close=True,
+    ):
         """
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
         excl : str | ExclusionMask
             Filepath to exclusions h5 or ExclusionMask file handler.
@@ -348,46 +385,56 @@
             A pre-loaded :class:`BespokeSinglePlantData` object, or
             ``None``. Can be useful to speed up execution on file
             systems with slow parallel reads.
         close : bool
             Flag to close object file handlers on exit.
         """
 
-        logger.debug('Initializing BespokeSinglePlant for gid {}...'
-                     .format(gid))
-        logger.debug('Resource filepath: {}'.format(res))
-        logger.debug('Exclusion filepath: {}'.format(excl))
-        logger.debug('Exclusion dict: {}'.format(excl_dict))
-        logger.debug('Bespoke objective function: {}'
-                     .format(objective_function))
-        logger.debug('Bespoke cost function: {}'.format(objective_function))
-        logger.debug('Bespoke wake loss multiplier: {}'
-                     .format(wake_loss_multiplier))
-        logger.debug('Bespoke GA initialization kwargs: {}'.format(ga_kwargs))
-        logger.debug('Bespoke EOS multiplier baseline capacity: {:,} MW'
-                     .format(eos_mult_baseline_cap_mw))
+        logger.debug(
+            "Initializing BespokeSinglePlant for gid {}...".format(gid)
+        )
+        logger.debug("Resource filepath: {}".format(res))
+        logger.debug("Exclusion filepath: {}".format(excl))
+        logger.debug("Exclusion dict: {}".format(excl_dict))
+        logger.debug(
+            "Bespoke objective function: {}".format(objective_function)
+        )
+        logger.debug("Bespoke cost function: {}".format(objective_function))
+        logger.debug(
+            "Bespoke wake loss multiplier: {}".format(wake_loss_multiplier)
+        )
+        logger.debug("Bespoke GA initialization kwargs: {}".format(ga_kwargs))
+        logger.debug(
+            "Bespoke EOS multiplier baseline capacity: {:,} MW".format(
+                eos_mult_baseline_cap_mw
+            )
+        )
 
-        if isinstance(min_spacing, str) and min_spacing.endswith('x'):
+        if isinstance(min_spacing, str) and min_spacing.endswith("x"):
             rotor_diameter = sam_sys_inputs["wind_turbine_rotor_diameter"]
-            min_spacing = float(min_spacing.strip('x')) * rotor_diameter
+            min_spacing = float(min_spacing.strip("x")) * rotor_diameter
 
         if not isinstance(min_spacing, (int, float)):
             try:
                 min_spacing = float(min_spacing)
             except Exception as e:
-                msg = ('min_spacing must be numeric but received: {}, {}'
-                       .format(min_spacing, type(min_spacing)))
+                msg = (
+                    "min_spacing must be numeric but received: {}, {}".format(
+                        min_spacing, type(min_spacing)
+                    )
+                )
                 logger.error(msg)
                 raise TypeError(msg) from e
 
         self.objective_function = objective_function
         self.capital_cost_function = capital_cost_function
         self.fixed_operating_cost_function = fixed_operating_cost_function
-        self.variable_operating_cost_function = \
+        self.variable_operating_cost_function = (
             variable_operating_cost_function
+        )
         self.min_spacing = min_spacing
         self.wake_loss_multiplier = wake_loss_multiplier
         self.ga_kwargs = ga_kwargs or {}
 
         self._sam_sys_inputs = sam_sys_inputs
         self._out_req = list(output_request)
         self._ws_bins = ws_bins
@@ -407,34 +454,41 @@
         self._bias_correct = Gen._parse_bc(bias_correct)
         self._pre_loaded_data = pre_loaded_data
         self._outputs = {}
 
         Handler = self.get_wind_handler(res)
         res = res if not isinstance(res, str) else Handler(res)
 
-        self._sc_point = AggSCPoint(gid, excl, res, tm_dset,
-                                    excl_dict=excl_dict,
-                                    inclusion_mask=inclusion_mask,
-                                    resolution=resolution,
-                                    excl_area=excl_area,
-                                    exclusion_shape=exclusion_shape,
-                                    close=close)
+        self._sc_point = AggSCPoint(
+            gid,
+            excl,
+            res,
+            tm_dset,
+            excl_dict=excl_dict,
+            inclusion_mask=inclusion_mask,
+            resolution=resolution,
+            excl_area=excl_area,
+            exclusion_shape=exclusion_shape,
+            close=close,
+        )
 
         self._parse_output_req()
         self._data_layers = data_layers
         self._parse_prior_run()
 
     def __str__(self):
-        s = ('BespokeSinglePlant for reV SC gid {} with resolution {}'
-             .format(self.sc_point.gid, self.sc_point.resolution))
+        s = "BespokeSinglePlant for reV SC gid {} with resolution {}".format(
+            self.sc_point.gid, self.sc_point.resolution
+        )
         return s
 
     def __repr__(self):
-        s = ('BespokeSinglePlant for reV SC gid {} with resolution {}'
-             .format(self.sc_point.gid, self.sc_point.resolution))
+        s = "BespokeSinglePlant for reV SC gid {} with resolution {}".format(
+            self.sc_point.gid, self.sc_point.resolution
+        )
         return s
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
@@ -443,65 +497,72 @@
 
     def _parse_output_req(self):
         """Make sure that the output request has basic important parameters
         (cf_mean, annual_energy) and process mean wind resource datasets
         (ws_mean, *_mean) if requested.
         """
 
-        required = ('cf_mean', 'annual_energy')
+        required = ("cf_mean", "annual_energy")
         for req in required:
             if req not in self._out_req:
                 self._out_req.append(req)
 
-        if 'ws_mean' in self._out_req:
-            self._out_req.remove('ws_mean')
-            self._outputs['ws_mean'] = self.res_df['windspeed'].mean()
+        if "ws_mean" in self._out_req:
+            self._out_req.remove("ws_mean")
+            self._outputs["ws_mean"] = self.res_df["windspeed"].mean()
 
         for req in copy.deepcopy(self._out_req):
             if req in self.res_df:
                 self._out_req.remove(req)
                 for annual_ti in self.annual_time_indexes:
                     year = annual_ti.year[0]
                     mask = self.res_df.index.isin(annual_ti)
                     arr = self.res_df.loc[mask, req].values.flatten()
-                    self._outputs[req + f'-{year}'] = arr
+                    self._outputs[req + f"-{year}"] = arr
 
-            elif req.replace('_mean', '') in self.res_df:
+            elif req.replace("_mean", "") in self.res_df:
                 self._out_req.remove(req)
-                dset = req.replace('_mean', '')
+                dset = req.replace("_mean", "")
                 self._outputs[req] = self.res_df[dset].mean()
 
-        if ('lcoe_fcr' in self._out_req
-                and 'fixed_charge_rate' not in self.original_sam_sys_inputs):
-            msg = ('User requested "lcoe_fcr" but did not input '
-                   '"fixed_charge_rate" in the SAM system config.')
+        if "lcoe_fcr" in self._out_req and (
+            "fixed_charge_rate" not in self.original_sam_sys_inputs
+        ):
+            msg = (
+                'User requested "lcoe_fcr" but did not input '
+                '"fixed_charge_rate" in the SAM system config.'
+            )
             logger.error(msg)
             raise KeyError(msg)
 
     def _parse_prior_run(self):
         """Parse prior bespoke wind plant optimization run meta data and make
         sure the SAM system inputs are set accordingly."""
 
         # {meta_column: sam_sys_input_key}
-        required = {'capacity': 'system_capacity',
-                    'turbine_x_coords': 'wind_farm_xCoordinates',
-                    'turbine_y_coords': 'wind_farm_yCoordinates'}
+        required = {
+            SupplyCurveField.CAPACITY: "system_capacity",
+            SupplyCurveField.TURBINE_X_COORDS: "wind_farm_xCoordinates",
+            SupplyCurveField.TURBINE_Y_COORDS: "wind_farm_yCoordinates",
+        }
 
         if self._prior_meta:
             missing = [k for k in required if k not in self.meta]
-            msg = ('Prior bespoke run meta data is missing the following '
-                   'required columns: {}'.format(missing))
+            msg = (
+                "Prior bespoke run meta data is missing the following "
+                "required columns: {}".format(missing)
+            )
             assert not any(missing), msg
 
             for meta_col, sam_sys_key in required.items():
                 prior_value = self.meta[meta_col].values[0]
                 self._sam_sys_inputs[sam_sys_key] = prior_value
 
             # convert reV supply curve cap in MW to SAM capacity in kW
-            self._sam_sys_inputs['system_capacity'] *= 1e3
+            self._sam_sys_inputs["system_capacity"] *= 1e3
 
     @staticmethod
     def _parse_gid_map(gid_map):
         """Parse the gid map and return the extracted dictionary or None if not
         provided
 
         Parameters
@@ -518,23 +579,30 @@
         Returns
         -------
         gid_map : dict | None
             Pre-extracted gid_map dictionary if provided or None if not.
         """
 
         if isinstance(gid_map, str):
-            if gid_map.endswith('.csv'):
-                gid_map = pd.read_csv(gid_map).to_dict()
-                assert 'gid' in gid_map, 'Need "gid" in gid_map column'
-                assert 'gid_map' in gid_map, 'Need "gid_map" in gid_map column'
-                gid_map = {gid_map['gid'][i]: gid_map['gid_map'][i]
-                           for i in gid_map['gid'].keys()}
+            if gid_map.endswith(".csv"):
+                gid_map = (
+                    pd.read_csv(gid_map)
+                    .rename(SupplyCurveField.map_to(ResourceMetaField), axis=1)
+                    .to_dict()
+                )
+                err_msg = f"Need {ResourceMetaField.GID} in gid_map column"
+                assert ResourceMetaField.GID in gid_map, err_msg
+                assert "gid_map" in gid_map, 'Need "gid_map" in gid_map column'
+                gid_map = {
+                    gid_map[ResourceMetaField.GID][i]: gid_map["gid_map"][i]
+                    for i in gid_map[ResourceMetaField.GID]
+                }
 
-            elif gid_map.endswith('.json'):
-                with open(gid_map, 'r') as f:
+            elif gid_map.endswith(".json"):
+                with open(gid_map) as f:
                     gid_map = json.load(f)
 
         return gid_map
 
     def close(self):
         """Close any open file handlers via the sc point attribute. If this
         class was initialized with close=False, this will not close any
@@ -559,27 +627,31 @@
 
         Returns
         -------
         ws : np.ndarray
             Bias corrected windspeed data in same shape as input
         """
 
-        if self._bias_correct is not None and dset.startswith('windspeed_'):
-
+        if self._bias_correct is not None and dset.startswith("windspeed_"):
             out = parse_bc_table(self._bias_correct, h5_gids)
             bc_fun, bc_fun_kwargs, bool_bc = out
 
             if bool_bc.any():
-                logger.debug('Bias correcting windspeed with function {} '
-                             'for h5 gids: {}'.format(bc_fun, h5_gids))
+                logger.debug(
+                    "Bias correcting windspeed with function {} "
+                    "for h5 gids: {}".format(bc_fun, h5_gids)
+                )
 
-                bc_fun_kwargs['ws'] = ws[:, bool_bc]
+                bc_fun_kwargs["ws"] = ws[:, bool_bc]
                 sig = signature(bc_fun)
-                bc_fun_kwargs = {k: v for k, v in bc_fun_kwargs.items()
-                                 if k in sig.parameters}
+                bc_fun_kwargs = {
+                    k: v
+                    for k, v in bc_fun_kwargs.items()
+                    if k in sig.parameters
+                }
 
                 ws[:, bool_bc] = bc_fun(**bc_fun_kwargs)
 
         return ws
 
     def get_weighted_res_ts(self, dset):
         """Special method for calculating the exclusion-weighted mean resource
@@ -627,15 +699,15 @@
         Returns
         -------
         mean_wind_dirs : np.ndarray
             Timeseries array of winddirection data in shape (n_time,) in units
             of degrees from north.
         """
 
-        dset = f'winddirection_{self.hub_height}m'
+        dset = f"winddirection_{self.hub_height}m"
         gids = self.sc_point.h5_gid_set
         h5_gids = copy.deepcopy(gids)
         if self._gid_map is not None:
             h5_gids = [self._gid_map[g] for g in gids]
 
         if self._pre_loaded_data is None:
             dirs = self.sc_point.h5[dset, :, h5_gids]
@@ -732,51 +804,56 @@
 
         Returns
         -------
         pd.DataFrame
         """
         if self._meta is None:
             res_gids = json.dumps([int(g) for g in self.sc_point.h5_gid_set])
-            gid_counts = json.dumps([float(np.round(n, 1))
-                                     for n in self.sc_point.gid_counts])
-
-            with SupplyCurveExtent(self.sc_point._excl_fpath,
-                                   resolution=self.sc_point.resolution) as sc:
+            gid_counts = json.dumps(
+                [float(np.round(n, 1)) for n in self.sc_point.gid_counts]
+            )
+
+            with SupplyCurveExtent(
+                self.sc_point._excl_fpath, resolution=self.sc_point.resolution
+            ) as sc:
                 row_ind, col_ind = sc.get_sc_row_col_ind(self.sc_point.gid)
 
             self._meta = pd.DataFrame(
-                {'sc_point_gid': self.sc_point.gid,
-                 'sc_row_ind': row_ind,
-                 'sc_col_ind': col_ind,
-                 'gid': self.sc_point.gid,
-                 'latitude': self.sc_point.latitude,
-                 'longitude': self.sc_point.longitude,
-                 'timezone': self.sc_point.timezone,
-                 'country': self.sc_point.country,
-                 'state': self.sc_point.state,
-                 'county': self.sc_point.county,
-                 'elevation': self.sc_point.elevation,
-                 'offshore': self.sc_point.offshore,
-                 'res_gids': res_gids,
-                 'gid_counts': gid_counts,
-                 'n_gids': self.sc_point.n_gids,
-                 'area_sq_km': self.sc_point.area,
-                 }, index=[self.sc_point.gid])
+                {
+                    SupplyCurveField.SC_POINT_GID: self.sc_point.gid,
+                    SupplyCurveField.SC_ROW_IND: row_ind,
+                    SupplyCurveField.SC_COL_IND: col_ind,
+                    SupplyCurveField.GID: self.sc_point.gid,
+                    SupplyCurveField.LATITUDE: self.sc_point.latitude,
+                    SupplyCurveField.LONGITUDE: self.sc_point.longitude,
+                    SupplyCurveField.TIMEZONE: self.sc_point.timezone,
+                    SupplyCurveField.COUNTRY: self.sc_point.country,
+                    SupplyCurveField.STATE: self.sc_point.state,
+                    SupplyCurveField.COUNTY: self.sc_point.county,
+                    SupplyCurveField.ELEVATION: self.sc_point.elevation,
+                    SupplyCurveField.OFFSHORE: self.sc_point.offshore,
+                    SupplyCurveField.RES_GIDS: res_gids,
+                    SupplyCurveField.GID_COUNTS: gid_counts,
+                    SupplyCurveField.N_GIDS: self.sc_point.n_gids,
+                    SupplyCurveField.AREA_SQ_KM: self.sc_point.area,
+                },
+                index=[self.sc_point.gid],
+            )
 
         return self._meta
 
     @property
     def hub_height(self):
         """Get the integer SAM system config turbine hub height (meters)
 
         Returns
         -------
         int
         """
-        return int(self.sam_sys_inputs['wind_turbine_hub_ht'])
+        return int(self.sam_sys_inputs["wind_turbine_hub_ht"])
 
     @property
     def res_df(self):
         """Get the reV compliant wind resource dataframe representing the
         aggregated and included wind resource in the current reV supply curve
         point at the turbine hub height. Includes a DatetimeIndex and columns
         for temperature, pressure, windspeed, and winddirection.
@@ -788,29 +865,34 @@
         if self._res_df is None:
             if self._pre_loaded_data is None:
                 ti = self.sc_point.h5.time_index
             else:
                 ti = self._pre_loaded_data.time_index
 
             wd = self.get_weighted_res_dir()
-            ws = self.get_weighted_res_ts(f'windspeed_{self.hub_height}m')
-            temp = self.get_weighted_res_ts(f'temperature_{self.hub_height}m')
-            pres = self.get_weighted_res_ts(f'pressure_{self.hub_height}m')
+            ws = self.get_weighted_res_ts(f"windspeed_{self.hub_height}m")
+            temp = self.get_weighted_res_ts(f"temperature_{self.hub_height}m")
+            pres = self.get_weighted_res_ts(f"pressure_{self.hub_height}m")
 
             # convert mbar to atm
             if np.nanmax(pres) > 1000:
                 pres *= 9.86923e-6
 
-            self._res_df = pd.DataFrame({'temperature': temp,
-                                         'pressure': pres,
-                                         'windspeed': ws,
-                                         'winddirection': wd}, index=ti)
+            self._res_df = pd.DataFrame(
+                {
+                    "temperature": temp,
+                    "pressure": pres,
+                    "windspeed": ws,
+                    "winddirection": wd,
+                },
+                index=ti,
+            )
 
-            if 'time_index_step' in self.original_sam_sys_inputs:
-                ti_step = self.original_sam_sys_inputs['time_index_step']
+            if "time_index_step" in self.original_sam_sys_inputs:
+                ti_step = self.original_sam_sys_inputs["time_index_step"]
                 self._res_df = self._res_df.iloc[::ti_step]
 
         return self._res_df
 
     @property
     def years(self):
         """Get the sorted list of analysis years.
@@ -853,17 +935,19 @@
             1D array of winddirections (deg) values that set the bin edges
             for the wind probability dist. Same len as wind_dist.shape[1] + 1
         """
         if self._wind_dist is None:
             ws_bins = JointPD._make_bins(*self._ws_bins)
             wd_bins = JointPD._make_bins(*self._wd_bins)
 
-            hist_out = np.histogram2d(self.res_df['windspeed'],
-                                      self.res_df['winddirection'],
-                                      bins=(ws_bins, wd_bins))
+            hist_out = np.histogram2d(
+                self.res_df["windspeed"],
+                self.res_df["winddirection"],
+                bins=(ws_bins, wd_bins),
+            )
             self._wind_dist, self._ws_edges, self._wd_edges = hist_out
             self._wind_dist /= self._wind_dist.sum()
 
         return self._wind_dist, self._ws_edges, self._wd_edges
 
     def initialize_wind_plant_ts(self):
         """Initialize the annual wind plant timeseries analysis object(s) using
@@ -876,44 +960,50 @@
             Annual reV.SAM.generation.WindPower object(s) keyed by year.
         """
         wind_plant_ts = {}
         for year in self.years:
             res_df = self.res_df[(self.res_df.index.year == year)]
             sam_inputs = copy.deepcopy(self.sam_sys_inputs)
 
-            if 'lcoe_fcr' in self._out_req:
+            if "lcoe_fcr" in self._out_req:
                 lcoe_kwargs = self.get_lcoe_kwargs()
                 sam_inputs.update(lcoe_kwargs)
 
-            i_wp = WindPower(res_df, self.meta, sam_inputs,
-                             output_request=self._out_req)
+            i_wp = WindPower(
+                res_df, self.meta, sam_inputs, output_request=self._out_req
+            )
             wind_plant_ts[year] = i_wp
 
         return wind_plant_ts
 
     @property
     def wind_plant_pd(self):
-        """reV WindPowerPD compute object for plant layout optimization based
+        """ReV WindPowerPD compute object for plant layout optimization based
         on wind joint probability distribution
 
         Returns
         -------
         reV.SAM.generation.WindPowerPD
         """
 
         if self._wind_plant_pd is None:
             wind_dist, ws_edges, wd_edges = self.wind_dist
-            self._wind_plant_pd = WindPowerPD(ws_edges, wd_edges, wind_dist,
-                                              self.meta, self.sam_sys_inputs,
-                                              output_request=self._out_req)
+            self._wind_plant_pd = WindPowerPD(
+                ws_edges,
+                wd_edges,
+                wind_dist,
+                self.meta,
+                self.sam_sys_inputs,
+                output_request=self._out_req,
+            )
         return self._wind_plant_pd
 
     @property
     def wind_plant_ts(self):
-        """reV WindPower compute object(s) based on wind resource timeseries
+        """ReV WindPower compute object(s) based on wind resource timeseries
         data keyed by year
 
         Returns
         -------
         dict
         """
         return self._wind_plant_ts
@@ -925,47 +1015,51 @@
         Returns
         -------
         PlaceTurbines
         """
         if self._plant_optm is None:
             # put import here to delay breaking due to special dependencies
             from reV.bespoke.place_turbines import PlaceTurbines
+
             self._plant_optm = PlaceTurbines(
                 self.wind_plant_pd,
                 self.objective_function,
                 self.capital_cost_function,
                 self.fixed_operating_cost_function,
                 self.variable_operating_cost_function,
                 self.include_mask,
                 self.pixel_side_length,
                 self.min_spacing,
-                self.wake_loss_multiplier)
+                self.wake_loss_multiplier,
+            )
 
         return self._plant_optm
 
     def recalc_lcoe(self):
         """Recalculate the multi-year mean LCOE based on the multi-year mean
         annual energy production (AEP)"""
 
-        if 'lcoe_fcr-means' in self.outputs:
+        if "lcoe_fcr-means" in self.outputs:
             lcoe_kwargs = self.get_lcoe_kwargs()
 
-            logger.debug('Recalulating multi-year mean LCOE using '
-                         'multi-year mean AEP.')
-
-            fcr = lcoe_kwargs['fixed_charge_rate']
-            cap_cost = lcoe_kwargs['capital_cost']
-            foc = lcoe_kwargs['fixed_operating_cost']
-            voc = lcoe_kwargs['variable_operating_cost']
-            aep = self.outputs['annual_energy-means']
+            logger.debug(
+                "Recalulating multi-year mean LCOE using "
+                "multi-year mean AEP."
+            )
+
+            fcr = lcoe_kwargs["fixed_charge_rate"]
+            cap_cost = lcoe_kwargs["capital_cost"]
+            foc = lcoe_kwargs["fixed_operating_cost"]
+            voc = lcoe_kwargs["variable_operating_cost"]
+            aep = self.outputs["annual_energy-means"]
 
             my_mean_lcoe = lcoe_fcr(fcr, cap_cost, foc, aep, voc)
 
-            self._outputs['lcoe_fcr-means'] = my_mean_lcoe
-            self._meta['mean_lcoe'] = my_mean_lcoe
+            self._outputs["lcoe_fcr-means"] = my_mean_lcoe
+            self._meta[SupplyCurveField.MEAN_LCOE] = my_mean_lcoe
 
     def get_lcoe_kwargs(self):
         """Get a namespace of arguments for calculating LCOE based on the
         bespoke optimized wind plant capacity
 
         Returns
         -------
@@ -975,16 +1069,21 @@
             updated based on the bespoke optimized system_capacity, includes
             fixed_charge_rate, system_capacity (kW), capital_cost ($),
             fixed_operating_cos ($), variable_operating_cost ($/kWh)
             Data source priority: outputs, plant_optimizer,
             original_sam_sys_inputs, meta
         """
 
-        kwargs_list = ['fixed_charge_rate', 'system_capacity', 'capital_cost',
-                       'fixed_operating_cost', 'variable_operating_cost']
+        kwargs_list = [
+            "fixed_charge_rate",
+            "system_capacity",
+            "capital_cost",
+            "fixed_operating_cost",
+            "variable_operating_cost",
+        ]
         lcoe_kwargs = {}
 
         for kwarg in kwargs_list:
             if kwarg in self.outputs:
                 lcoe_kwargs[kwarg] = self.outputs[kwarg]
             elif getattr(self.plant_optimizer, kwarg, None) is not None:
                 lcoe_kwargs[kwarg] = getattr(self.plant_optimizer, kwarg)
@@ -995,17 +1094,20 @@
                 lcoe_kwargs[kwarg] = value
 
         for k, v in lcoe_kwargs.items():
             self._meta[k] = v
 
         missing = [k for k in kwargs_list if k not in lcoe_kwargs]
         if any(missing):
-            msg = ('Could not find these LCOE kwargs in outputs, '
-                   'plant_optimizer, original_sam_sys_inputs, or meta: {}'
-                   .format(missing))
+            msg = (
+                "Could not find these LCOE kwargs in outputs, "
+                "plant_optimizer, original_sam_sys_inputs, or meta: {}".format(
+                    missing
+                )
+            )
             logger.error(msg)
             raise KeyError(msg)
 
         return lcoe_kwargs
 
     @staticmethod
     def get_wind_handler(res):
@@ -1020,15 +1122,15 @@
         Returns
         -------
         handler : WindResource | MultiYearWindResource
             Wind resource handler or multi year handler
         """
         handler = res
         if isinstance(res, str):
-            if '*' in res:
+            if "*" in res:
                 handler = MultiYearWindResource
             else:
                 handler = WindResource
         return handler
 
     @classmethod
     def check_dependencies(cls):
@@ -1038,45 +1140,52 @@
         for name in cls.DEPENDENCIES:
             try:
                 import_module(name)
             except ModuleNotFoundError:
                 missing.append(name)
 
         if any(missing):
-            msg = ('The reV bespoke module depends on the following special '
-                   'dependencies that were not found in the active '
-                   'environment: {}'.format(missing))
+            msg = (
+                "The reV bespoke module depends on the following special "
+                "dependencies that were not found in the active "
+                "environment: {}".format(missing)
+            )
             logger.error(msg)
             raise ModuleNotFoundError(msg)
 
     @staticmethod
-    def _check_sys_inputs(plant1, plant2,
-                          ignore=('wind_resource_model_choice',
-                                  'wind_resource_data',
-                                  'wind_turbine_powercurve_powerout',
-                                  'hourly',
-                                  'capital_cost',
-                                  'fixed_operating_cost',
-                                  'variable_operating_cost')):
+    def _check_sys_inputs(
+        plant1,
+        plant2,
+        ignore=(
+            "wind_resource_model_choice",
+            "wind_resource_data",
+            "wind_turbine_powercurve_powerout",
+            "hourly",
+            "capital_cost",
+            "fixed_operating_cost",
+            "variable_operating_cost",
+        ),
+    ):
         """Check two reV-SAM models for matching system inputs.
 
         Parameters
         ----------
         plant1/plant2 : reV.SAM.generation.WindPower
             Two WindPower analysis objects to check.
         """
         bad = []
         for k, v in plant1.sam_sys_inputs.items():
-            if k not in plant2.sam_sys_inputs:
-                bad.append(k)
-            elif str(v) != str(plant2.sam_sys_inputs[k]):
+            if k not in plant2.sam_sys_inputs or str(v) != str(
+                plant2.sam_sys_inputs[k]
+            ):
                 bad.append(k)
         bad = [b for b in bad if b not in ignore]
         if any(bad):
-            msg = 'Inputs no longer match: {}'.format(bad)
+            msg = "Inputs no longer match: {}".format(bad)
             logger.error(msg)
             raise RuntimeError(msg)
 
     def run_wind_plant_ts(self):
         """Run the wind plant multi-year timeseries analysis and export output
         requests to outputs property.
 
@@ -1084,49 +1193,59 @@
         -------
         outputs : dict
             Output dictionary for the full BespokeSinglePlant object. The
             multi-year timeseries data is also exported to the
             BespokeSinglePlant.outputs property.
         """
 
-        logger.debug('Running {} years of SAM timeseries analysis for {}'
-                     .format(len(self.years), self))
+        logger.debug(
+            "Running {} years of SAM timeseries analysis for {}".format(
+                len(self.years), self
+            )
+        )
         self._wind_plant_ts = self.initialize_wind_plant_ts()
         for year, plant in self.wind_plant_ts.items():
             self._check_sys_inputs(plant, self.wind_plant_pd)
             try:
                 plant.run_gen_and_econ()
             except Exception as e:
-                msg = ('{} failed while trying to run SAM WindPower '
-                       'timeseries analysis for {}'.format(self, year))
+                msg = (
+                    "{} failed while trying to run SAM WindPower "
+                    "timeseries analysis for {}".format(self, year)
+                )
                 logger.exception(msg)
                 raise RuntimeError(msg) from e
 
             for k, v in plant.outputs.items():
-                self._outputs[k + '-{}'.format(year)] = v
+                self._outputs[k + "-{}".format(year)] = v
 
         means = {}
         for k1, v1 in self._outputs.items():
-            if isinstance(v1, Number) and parse_year(k1, option='boolean'):
+            if isinstance(v1, Number) and parse_year(k1, option="boolean"):
                 year = parse_year(k1)
-                base_str = k1.replace(str(year), '')
-                all_values = [v2 for k2, v2 in self._outputs.items()
-                              if base_str in k2]
-                means[base_str + 'means'] = np.mean(all_values)
+                base_str = k1.replace(str(year), "")
+                all_values = [
+                    v2 for k2, v2 in self._outputs.items() if base_str in k2
+                ]
+                means[base_str + "means"] = np.mean(all_values)
 
         self._outputs.update(means)
 
         # copy dataset outputs to meta data for supply curve table summary
-        if 'cf_mean-means' in self.outputs:
-            self._meta.loc[:, 'mean_cf'] = self.outputs['cf_mean-means']
-        if 'lcoe_fcr-means' in self.outputs:
-            self._meta.loc[:, 'mean_lcoe'] = self.outputs['lcoe_fcr-means']
+        if "cf_mean-means" in self.outputs:
+            self._meta.loc[:, SupplyCurveField.MEAN_CF] = self.outputs[
+                "cf_mean-means"
+            ]
+        if "lcoe_fcr-means" in self.outputs:
+            self._meta.loc[:, SupplyCurveField.MEAN_LCOE] = self.outputs[
+                "lcoe_fcr-means"
+            ]
             self.recalc_lcoe()
 
-        logger.debug('Timeseries analysis complete!')
+        logger.debug("Timeseries analysis complete!")
 
         return self.outputs
 
     def run_plant_optimization(self):
         """Run the wind plant layout optimization and export outputs
         to outputs property.
 
@@ -1134,21 +1253,22 @@
         -------
         outputs : dict
             Output dictionary for the full BespokeSinglePlant object. The
             layout optimization output data is also exported to the
             BespokeSinglePlant.outputs property.
         """
 
-        logger.debug('Running plant layout optimization for {}'.format(self))
+        logger.debug("Running plant layout optimization for {}".format(self))
         try:
             self.plant_optimizer.place_turbines(**self.ga_kwargs)
         except Exception as e:
-            msg = ('{} failed while trying to run the '
-                   'turbine placement optimizer'
-                   .format(self))
+            msg = (
+                "{} failed while trying to run the "
+                "turbine placement optimizer".format(self)
+            )
             logger.exception(msg)
             raise RuntimeError(msg) from e
 
         # TODO need to add:
         # total cell area
         # cell capacity density
 
@@ -1158,70 +1278,84 @@
         pyc = [int(np.round(c)) for c in self.plant_optimizer.y_locations]
 
         txc = json.dumps(txc)
         tyc = json.dumps(tyc)
         pxc = json.dumps(pxc)
         pyc = json.dumps(pyc)
 
-        self._meta["turbine_x_coords"] = txc
-        self._meta["turbine_y_coords"] = tyc
+        self._meta[SupplyCurveField.TURBINE_X_COORDS] = txc
+        self._meta[SupplyCurveField.TURBINE_Y_COORDS] = tyc
         self._meta["possible_x_coords"] = pxc
         self._meta["possible_y_coords"] = pyc
 
         self._outputs["full_polygons"] = self.plant_optimizer.full_polygons
-        self._outputs["packing_polygons"] = \
+        self._outputs["packing_polygons"] = (
             self.plant_optimizer.packing_polygons
+        )
         self._outputs["system_capacity"] = self.plant_optimizer.capacity
 
         self._meta["n_turbines"] = self.plant_optimizer.nturbs
         self._meta["bespoke_aep"] = self.plant_optimizer.aep
         self._meta["bespoke_objective"] = self.plant_optimizer.objective
-        self._meta["bespoke_capital_cost"] = \
-            self.plant_optimizer.capital_cost
-        self._meta["bespoke_fixed_operating_cost"] = \
+        self._meta["bespoke_capital_cost"] = self.plant_optimizer.capital_cost
+        self._meta["bespoke_fixed_operating_cost"] = (
             self.plant_optimizer.fixed_operating_cost
-        self._meta["bespoke_variable_operating_cost"] = \
+        )
+        self._meta["bespoke_variable_operating_cost"] = (
             self.plant_optimizer.variable_operating_cost
+        )
         self._meta["included_area"] = self.plant_optimizer.area
-        self._meta["included_area_capacity_density"] = \
+        self._meta["included_area_capacity_density"] = (
             self.plant_optimizer.capacity_density
-        self._meta["convex_hull_area"] = \
-            self.plant_optimizer.convex_hull_area
-        self._meta["convex_hull_capacity_density"] = \
+        )
+        self._meta["convex_hull_area"] = self.plant_optimizer.convex_hull_area
+        self._meta["convex_hull_capacity_density"] = (
             self.plant_optimizer.convex_hull_capacity_density
-        self._meta["full_cell_capacity_density"] = \
+        )
+        self._meta["full_cell_capacity_density"] = (
             self.plant_optimizer.full_cell_capacity_density
+        )
 
-        logger.debug('Plant layout optimization complete!')
+        logger.debug("Plant layout optimization complete!")
 
         # copy dataset outputs to meta data for supply curve table summary
         # convert SAM system capacity in kW to reV supply curve cap in MW
-        self._meta['capacity'] = self.outputs['system_capacity'] / 1e3
+        self._meta[SupplyCurveField.CAPACITY] = (
+            self.outputs["system_capacity"] / 1e3
+        )
 
         # add required ReEDS multipliers to meta
         baseline_cost = self.plant_optimizer.capital_cost_per_kw(
-            capacity_mw=self._baseline_cap_mw)
-        self._meta['eos_mult'] = (self.plant_optimizer.capital_cost
-                                  / self.plant_optimizer.capacity
-                                  / baseline_cost)
-        self._meta['reg_mult'] = (self.sam_sys_inputs
-                                  .get("capital_cost_multiplier", 1))
+            capacity_mw=self._baseline_cap_mw
+        )
+        self._meta[SupplyCurveField.EOS_MULT] = (
+            self.plant_optimizer.capital_cost
+            / self.plant_optimizer.capacity
+            / baseline_cost
+        )
+        self._meta[SupplyCurveField.REG_MULT] = self.sam_sys_inputs.get(
+            "capital_cost_multiplier", 1
+        )
 
         return self.outputs
 
     def agg_data_layers(self):
         """Aggregate optional data layers if requested and save to self.meta"""
         if self._data_layers is not None:
-            logger.debug('Aggregating {} extra data layers.'
-                         .format(len(self._data_layers)))
+            logger.debug(
+                "Aggregating {} extra data layers.".format(
+                    len(self._data_layers)
+                )
+            )
             point_summary = self.meta.to_dict()
-            point_summary = self.sc_point.agg_data_layers(point_summary,
-                                                          self._data_layers)
+            point_summary = self.sc_point.agg_data_layers(
+                point_summary, self._data_layers
+            )
             self._meta = pd.DataFrame(point_summary)
-            logger.debug('Finished aggregating extra data layers.')
+            logger.debug("Finished aggregating extra data layers.")
 
     @property
     def outputs(self):
         """Saved outputs for the single wind plant bespoke optimization.
 
         Returns
         -------
@@ -1242,46 +1376,66 @@
         bsp : dict
             Bespoke single plant outputs namespace keyed by dataset name
             including a dataset "meta" for the BespokeSinglePlant meta data.
         """
 
         with cls(*args, **kwargs) as bsp:
             if bsp._prior_meta:
-                logger.debug('Skipping bespoke plant optimization for gid {}. '
-                             'Received prior meta data for this point.'
-                             .format(bsp.gid))
+                logger.debug(
+                    "Skipping bespoke plant optimization for gid {}. "
+                    "Received prior meta data for this point.".format(bsp.gid)
+                )
             else:
                 _ = bsp.run_plant_optimization()
 
             _ = bsp.run_wind_plant_ts()
             bsp.agg_data_layers()
 
             meta = bsp.meta
             out = bsp.outputs
-            out['meta'] = meta
+            out["meta"] = meta
             for year, ti in zip(bsp.years, bsp.annual_time_indexes):
-                out['time_index-{}'.format(year)] = ti
+                out["time_index-{}".format(year)] = ti
 
         return out
 
 
 class BespokeWindPlants(BaseAggregation):
     """BespokeWindPlants"""
 
-    def __init__(self, excl_fpath, res_fpath, tm_dset, objective_function,
-                 capital_cost_function, fixed_operating_cost_function,
-                 variable_operating_cost_function, project_points,
-                 sam_files, min_spacing='5x', wake_loss_multiplier=1,
-                 ga_kwargs=None, output_request=('system_capacity', 'cf_mean'),
-                 ws_bins=(0.0, 20.0, 5.0), wd_bins=(0.0, 360.0, 45.0),
-                 excl_dict=None, area_filter_kernel='queen', min_area=None,
-                 resolution=64, excl_area=None, data_layers=None,
-                 pre_extract_inclusions=False, prior_run=None, gid_map=None,
-                 bias_correct=None, pre_load_data=False):
-        """reV bespoke analysis class.
+    def __init__(
+        self,
+        excl_fpath,
+        res_fpath,
+        tm_dset,
+        objective_function,
+        capital_cost_function,
+        fixed_operating_cost_function,
+        variable_operating_cost_function,
+        project_points,
+        sam_files,
+        min_spacing="5x",
+        wake_loss_multiplier=1,
+        ga_kwargs=None,
+        output_request=("system_capacity", "cf_mean"),
+        ws_bins=(0.0, 20.0, 5.0),
+        wd_bins=(0.0, 360.0, 45.0),
+        excl_dict=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        resolution=64,
+        excl_area=None,
+        data_layers=None,
+        pre_extract_inclusions=False,
+        prior_run=None,
+        gid_map=None,
+        bias_correct=None,
+        pre_load_data=False,
+    ):
+        r"""ReV bespoke analysis class.
 
         Much like generation, ``reV`` bespoke analysis runs SAM
         simulations by piping in renewable energy resource data (usually
         from the WTK), loading the SAM config, and then executing the
         :py:class:`PySAM.Windpower.Windpower` compute module.
         However, unlike ``reV`` generation, bespoke analysis is
         performed on the supply-curve grid resolution, and the plant
@@ -1681,47 +1835,66 @@
             significant amount of RAM, so be sure to split execution
             across many nodes (e.g. 100 nodes, 36 workers each for
             CONUS) or request large amounts of memory for a smaller
             number of nodes. By default, ``False``.
         """
 
         log_versions(logger)
-        logger.info('Initializing BespokeWindPlants...')
-        logger.info('Resource filepath: {}'.format(res_fpath))
-        logger.info('Exclusion filepath: {}'.format(excl_fpath))
-        logger.debug('Exclusion dict: {}'.format(excl_dict))
-        logger.info('Bespoke objective function: {}'
-                    .format(objective_function))
-        logger.info('Bespoke capital cost function: {}'
-                    .format(capital_cost_function))
-        logger.info('Bespoke fixed operating cost function: {}'
-                    .format(fixed_operating_cost_function))
-        logger.info('Bespoke variable operating cost function: {}'
-                    .format(variable_operating_cost_function))
-        logger.info('Bespoke wake loss multiplier: {}'
-                    .format(wake_loss_multiplier))
-        logger.info('Bespoke GA initialization kwargs: {}'.format(ga_kwargs))
-
-        logger.info('Bespoke pre-extracting exclusions: {}'
-                    .format(pre_extract_inclusions))
-        logger.info('Bespoke pre-extracting resource data: {}'
-                    .format(pre_load_data))
-        logger.info('Bespoke prior run: {}'.format(prior_run))
-        logger.info('Bespoke GID map: {}'.format(gid_map))
-        logger.info('Bespoke bias correction table: {}'.format(bias_correct))
+        logger.info("Initializing BespokeWindPlants...")
+        logger.info("Resource filepath: {}".format(res_fpath))
+        logger.info("Exclusion filepath: {}".format(excl_fpath))
+        logger.debug("Exclusion dict: {}".format(excl_dict))
+        logger.info(
+            "Bespoke objective function: {}".format(objective_function)
+        )
+        logger.info(
+            "Bespoke capital cost function: {}".format(capital_cost_function)
+        )
+        logger.info(
+            "Bespoke fixed operating cost function: {}".format(
+                fixed_operating_cost_function
+            )
+        )
+        logger.info(
+            "Bespoke variable operating cost function: {}".format(
+                variable_operating_cost_function
+            )
+        )
+        logger.info(
+            "Bespoke wake loss multiplier: {}".format(wake_loss_multiplier)
+        )
+        logger.info("Bespoke GA initialization kwargs: {}".format(ga_kwargs))
+
+        logger.info(
+            "Bespoke pre-extracting exclusions: {}".format(
+                pre_extract_inclusions
+            )
+        )
+        logger.info(
+            "Bespoke pre-extracting resource data: {}".format(pre_load_data)
+        )
+        logger.info("Bespoke prior run: {}".format(prior_run))
+        logger.info("Bespoke GID map: {}".format(gid_map))
+        logger.info("Bespoke bias correction table: {}".format(bias_correct))
 
         BespokeSinglePlant.check_dependencies()
 
         self._project_points = self._parse_points(project_points, sam_files)
 
-        super().__init__(excl_fpath, tm_dset, excl_dict=excl_dict,
-                         area_filter_kernel=area_filter_kernel,
-                         min_area=min_area, resolution=resolution,
-                         excl_area=excl_area, gids=self._project_points.gids,
-                         pre_extract_inclusions=pre_extract_inclusions)
+        super().__init__(
+            excl_fpath,
+            tm_dset,
+            excl_dict=excl_dict,
+            area_filter_kernel=area_filter_kernel,
+            min_area=min_area,
+            resolution=resolution,
+            excl_area=excl_area,
+            gids=self._project_points.gids,
+            pre_extract_inclusions=pre_extract_inclusions,
+        )
 
         self._res_fpath = res_fpath
         self._obj_fun = objective_function
         self._cap_cost_fun = capital_cost_function
         self._foc_fun = fixed_operating_cost_function
         self._voc_fun = variable_operating_cost_function
         self._min_spacing = min_spacing
@@ -1738,44 +1911,52 @@
         self._check_files()
 
         self._pre_loaded_data = None
         self._pre_load_data(pre_load_data)
 
         self._slice_lookup = None
 
-        logger.info('Initialized BespokeWindPlants with project points: {}'
-                    .format(self._project_points))
+        logger.info(
+            "Initialized BespokeWindPlants with project points: {}".format(
+                self._project_points
+            )
+        )
 
     @staticmethod
     def _parse_points(points, sam_configs):
         """Parse a project points object using a project points file
 
         Parameters
         ----------
         points : int | slice | list | str | PointsControl | None
             Slice or list specifying project points, string pointing to a
             project points csv, or a fully instantiated PointsControl object.
             Can also be a single site integer value. Points csv should have
-            'gid' and 'config' column, the config maps to the sam_configs dict
-            keys.
+            `SupplyCurveField.GID` and 'config' column, the config maps to the
+            sam_configs dict keys.
         sam_configs : dict | str | SAMConfig
             SAM input configuration ID(s) and file path(s). Keys are the SAM
             config ID(s) which map to the config column in the project points
             CSV. Values are either a JSON SAM config file or dictionary of SAM
             config inputs. Can also be a single config file path or a
             pre loaded SAMConfig object.
 
         Returns
         -------
         ProjectPoints : ~reV.config.project_points.ProjectPoints
             Project points object laying out the supply curve gids to
             analyze.
         """
-        pc = Gen.get_pc(points, points_range=None, sam_configs=sam_configs,
-                        tech='windpower', sites_per_worker=1)
+        pc = Gen.get_pc(
+            points,
+            points_range=None,
+            sam_configs=sam_configs,
+            tech="windpower",
+            sites_per_worker=1,
+        )
 
         return pc.project_points
 
     @staticmethod
     def _parse_prior_run(prior_run):
         """Extract bespoke meta data from prior run and verify that the run is
         compatible with the new job specs.
@@ -1797,23 +1978,23 @@
             columns will be json loaded.
         """
 
         meta = None
 
         if prior_run is not None:
             assert os.path.isfile(prior_run)
-            assert prior_run.endswith('.h5')
+            assert prior_run.endswith(".h5")
 
-            with Outputs(prior_run, mode='r') as f:
+            with Outputs(prior_run, mode="r") as f:
                 meta = f.meta
 
             # pylint: disable=no-member
             for col in meta.columns:
                 val = meta[col].values[0]
-                if isinstance(val, str) and val[0] == '[' and val[-1] == ']':
+                if isinstance(val, str) and val[0] == "[" and val[-1] == "]":
                     meta[col] = meta[col].apply(json.loads)
 
         return meta
 
     def _get_prior_meta(self, gid):
         """Get the meta data for a given gid from the prior run (if available)
 
@@ -1826,15 +2007,15 @@
         -------
         meta : pd.DataFrame
             Prior meta data for just the requested gid.
         """
         meta = None
 
         if self._prior_meta is not None:
-            mask = self._prior_meta['gid'] == gid
+            mask = self._prior_meta[SupplyCurveField.GID] == gid
             if any(mask):
                 meta = self._prior_meta[mask]
 
         return meta
 
     def _check_files(self):
         """Do a preflight check on input files"""
@@ -1842,67 +2023,79 @@
         paths = self._excl_fpath
         if isinstance(self._excl_fpath, str):
             paths = [self._excl_fpath]
 
         for path in paths:
             if not os.path.exists(path):
                 raise FileNotFoundError(
-                    'Could not find required exclusions file: '
-                    '{}'.format(path))
+                    "Could not find required exclusions file: " "{}".format(
+                        path
+                    )
+                )
 
         with ExclusionLayers(paths) as excl:
             if self._tm_dset not in excl:
-                raise FileInputError('Could not find techmap dataset "{}" '
-                                     'in the exclusions file(s): {}'
-                                     .format(self._tm_dset, paths))
+                raise FileInputError(
+                    'Could not find techmap dataset "{}" '
+                    "in the exclusions file(s): {}".format(
+                        self._tm_dset, paths
+                    )
+                )
 
         # just check that this file exists, cannot check res_fpath if *glob
         Handler = BespokeSinglePlant.get_wind_handler(self._res_fpath)
         with Handler(self._res_fpath) as f:
             assert any(f.dsets)
 
     def _pre_load_data(self, pre_load_data):
-        """Pre-load resource data, if requested. """
+        """Pre-load resource data, if requested."""
         if not pre_load_data:
             return
 
-        sc_gid_to_hh = {gid: self._hh_for_sc_gid(gid)
-                        for gid in self._project_points.df["gid"]}
+        sc_gid_to_hh = {
+            gid: self._hh_for_sc_gid(gid)
+            for gid in self._project_points.df[ResourceMetaField.GID]
+        }
 
         with ExclusionLayers(self._excl_fpath) as excl:
             tm = excl[self._tm_dset]
 
         scp_kwargs = {"shape": self.shape, "resolution": self._resolution}
-        slices = {gid: SupplyCurvePoint.get_agg_slices(gid=gid, **scp_kwargs)
-                  for gid in self._project_points.df["gid"]}
-
-        sc_gid_to_res_gid = {gid: sorted(set(tm[slx, sly].flatten()))
-                             for gid, (slx, sly) in slices.items()}
+        slices = {
+            gid: SupplyCurvePoint.get_agg_slices(gid=gid, **scp_kwargs)
+            for gid in self._project_points.df[ResourceMetaField.GID]
+        }
+
+        sc_gid_to_res_gid = {
+            gid: sorted(set(tm[slx, sly].flatten()))
+            for gid, (slx, sly) in slices.items()
+        }
 
         for sc_gid, res_gids in sc_gid_to_res_gid.items():
             if res_gids[0] < 0:
                 sc_gid_to_res_gid[sc_gid] = res_gids[1:]
 
         if self._gid_map is not None:
             for sc_gid, res_gids in sc_gid_to_res_gid.items():
-                sc_gid_to_res_gid[sc_gid] = sorted(self._gid_map[g]
-                                                   for g in res_gids)
+                sc_gid_to_res_gid[sc_gid] = sorted(
+                    self._gid_map[g] for g in res_gids
+                )
 
         logger.info("Pre-loading resource data for Bespoke run... ")
-        self._pre_loaded_data = BespokeMultiPlantData(self._res_fpath,
-                                                      sc_gid_to_hh,
-                                                      sc_gid_to_res_gid)
+        self._pre_loaded_data = BespokeMultiPlantData(
+            self._res_fpath, sc_gid_to_hh, sc_gid_to_res_gid
+        )
 
     def _hh_for_sc_gid(self, sc_gid):
         """Fetch the hh for a given sc_gid"""
         config = self.sam_sys_inputs_with_site_data(sc_gid)
         return int(config["wind_turbine_hub_ht"])
 
     def _pre_loaded_data_for_sc_gid(self, sc_gid):
-        """Pre-load data for a given SC GID, if requested. """
+        """Pre-load data for a given SC GID, if requested."""
         if self._pre_loaded_data is None:
             return None
 
         return self._pre_loaded_data.get_preloaded_data_for_gid(sc_gid)
 
     def _get_bc_for_gid(self, gid):
         """Get the bias correction table trimmed down just for the resource
@@ -1922,17 +2115,20 @@
             bias correction table that correspond to the SC point gid
         """
         out = self._bias_correct
 
         if self._bias_correct is not None:
             h5_gids = []
             try:
-                scp_kwargs = dict(gid=gid, excl=self._excl_fpath,
-                                  tm_dset=self._tm_dset,
-                                  resolution=self._resolution)
+                scp_kwargs = dict(
+                    gid=gid,
+                    excl=self._excl_fpath,
+                    tm_dset=self._tm_dset,
+                    resolution=self._resolution,
+                )
                 with SupplyCurvePoint(**scp_kwargs) as scp:
                     h5_gids = scp.h5_gid_set
             except EmptySupplyCurvePointError:
                 pass
 
             if self._gid_map is not None:
                 h5_gids = [self._gid_map[g] for g in h5_gids]
@@ -1968,27 +2164,28 @@
     def meta(self):
         """Meta data for all completed BespokeSinglePlant objects.
 
         Returns
         -------
         pd.DataFrame
         """
-        meta = [self.outputs[g]['meta'] for g in self.completed_gids]
+        meta = [self.outputs[g]["meta"] for g in self.completed_gids]
         if len(self.completed_gids) > 1:
             meta = pd.concat(meta, axis=0)
         else:
             meta = meta[0]
         return meta
 
     @property
     def slice_lookup(self):
-        """dict | None: Lookup mapping sc_point_gid to exclusion slice. """
+        """Dict | None: Lookup mapping sc_point_gid to exclusion slice."""
         if self._slice_lookup is None and self._inclusion_mask is not None:
-            with SupplyCurveExtent(self._excl_fpath,
-                                   resolution=self._resolution) as sc:
+            with SupplyCurveExtent(
+                self._excl_fpath, resolution=self._resolution
+            ) as sc:
                 assert self.shape == self._inclusion_mask.shape
                 self._slice_lookup = sc.get_slice_lookup(self.gids)
 
         return self._slice_lookup
 
     def sam_sys_inputs_with_site_data(self, gid):
         """Update the sam_sys_inputs with site data for the given GID.
@@ -2009,16 +2206,21 @@
             DataFrame.
         """
 
         gid_idx = self._project_points.index(gid)
         site_data = self._project_points.df.iloc[gid_idx]
 
         site_sys_inputs = self._project_points[gid][1]
-        site_sys_inputs.update({k: v for k, v in site_data.to_dict().items()
-                                if not (isinstance(v, float) and np.isnan(v))})
+        site_sys_inputs.update(
+            {
+                k: v
+                for k, v in site_data.to_dict().items()
+                if not (isinstance(v, float) and np.isnan(v))
+            }
+        )
         return site_sys_inputs
 
     def _init_fout(self, out_fpath, sample):
         """Initialize the bespoke output h5 file with meta and time index dsets
 
         Parameters
         ----------
@@ -2029,21 +2231,22 @@
             A single sample BespokeSinglePlant output dict that has been run
             and has output data.
         """
         out_dir = os.path.dirname(out_fpath)
         if not os.path.exists(out_dir):
             create_dirs(out_dir)
 
-        with Outputs(out_fpath, mode='w') as f:
-            f._set_meta('meta', self.meta, attrs={})
-            ti_dsets = [d for d in sample.keys()
-                        if d.startswith('time_index-')]
+        with Outputs(out_fpath, mode="w") as f:
+            f._set_meta("meta", self.meta, attrs={})
+            ti_dsets = [
+                d for d in sample.keys() if d.startswith("time_index-")
+            ]
             for dset in ti_dsets:
                 f._set_time_index(dset, sample[dset], attrs={})
-                f._set_time_index('time_index', sample[dset], attrs={})
+                f._set_time_index("time_index", sample[dset], attrs={})
 
     def _collect_out_arr(self, dset, sample):
         """Collect single-plant data arrays into complete arrays with data from
         all BespokeSinglePlant objects.
 
         Parameters
         ----------
@@ -2066,28 +2269,30 @@
         if isinstance(single_arr, Number):
             shape = (len(self.completed_gids),)
             sample_num = single_arr
         elif isinstance(single_arr, (list, tuple, np.ndarray)):
             shape = (len(single_arr), len(self.completed_gids))
             sample_num = single_arr[0]
         else:
-            msg = ('Not writing dataset "{}" of type "{}" to disk.'
-                   .format(dset, type(single_arr)))
+            msg = 'Not writing dataset "{}" of type "{}" to disk.'.format(
+                dset, type(single_arr)
+            )
             logger.info(msg)
             return None
 
         if isinstance(sample_num, float):
             dtype = np.float32
         else:
             dtype = type(sample_num)
         full_arr = np.zeros(shape, dtype=dtype)
 
         # collect data from all wind plants
-        logger.info('Collecting dataset "{}" with final shape {}'
-                    .format(dset, shape))
+        logger.info(
+            'Collecting dataset "{}" with final shape {}'.format(dset, shape)
+        )
         for i, gid in enumerate(self.completed_gids):
             if len(full_arr.shape) == 1:
                 full_arr[i] = self.outputs[gid][dset]
             else:
                 full_arr[:, i] = self.outputs[gid][dset]
 
         return full_arr
@@ -2103,74 +2308,96 @@
 
         Returns
         -------
         out_fpath : str
             Full filepath to desired .h5 output file, the .h5 extension has
             been added if it was not already present.
         """
-        if not out_fpath.endswith('.h5'):
-            out_fpath += '.h5'
+        if not out_fpath.endswith(".h5"):
+            out_fpath += ".h5"
 
         if ModuleName.BESPOKE not in out_fpath:
             extension_with_module = "_{}.h5".format(ModuleName.BESPOKE)
             out_fpath = out_fpath.replace(".h5", extension_with_module)
 
         if not self.completed_gids:
-            msg = ("No output data found! It is likely that all requested "
-                   "points are excluded.")
+            msg = (
+                "No output data found! It is likely that all requested "
+                "points are excluded."
+            )
             logger.warning(msg)
             warn(msg)
             return out_fpath
 
         sample = self.outputs[self.completed_gids[0]]
         self._init_fout(out_fpath, sample)
 
-        dsets = [d for d in sample.keys()
-                 if not d.startswith('time_index-')
-                 and d != 'meta']
-        with Outputs(out_fpath, mode='a') as f:
+        dsets = [
+            d
+            for d in sample.keys()
+            if not d.startswith("time_index-") and d != "meta"
+        ]
+        with Outputs(out_fpath, mode="a") as f:
             for dset in dsets:
                 full_arr = self._collect_out_arr(dset, sample)
                 if full_arr is not None:
                     dset_no_year = dset
-                    if parse_year(dset, option='boolean'):
+                    if parse_year(dset, option="boolean"):
                         year = parse_year(dset)
-                        dset_no_year = dset.replace('-{}'.format(year), '')
+                        dset_no_year = dset.replace("-{}".format(year), "")
 
                     attrs = BespokeSinglePlant.OUT_ATTRS.get(dset_no_year, {})
                     attrs = copy.deepcopy(attrs)
-                    dtype = attrs.pop('dtype', np.float32)
-                    chunks = attrs.pop('chunks', None)
+                    dtype = attrs.pop("dtype", np.float32)
+                    chunks = attrs.pop("chunks", None)
                     try:
-                        f.write_dataset(dset, full_arr, dtype, chunks=chunks,
-                                        attrs=attrs)
+                        f.write_dataset(
+                            dset, full_arr, dtype, chunks=chunks, attrs=attrs
+                        )
                     except Exception as e:
                         msg = 'Failed to write "{}" to disk.'.format(dset)
                         logger.exception(msg)
-                        raise IOError(msg) from e
+                        raise OSError(msg) from e
 
-        logger.info('Saved output data to: {}'.format(out_fpath))
+        logger.info("Saved output data to: {}".format(out_fpath))
         return out_fpath
 
     # pylint: disable=arguments-renamed
     @classmethod
-    def run_serial(cls, excl_fpath, res_fpath, tm_dset,
-                   sam_sys_inputs, objective_function,
-                   capital_cost_function,
-                   fixed_operating_cost_function,
-                   variable_operating_cost_function,
-                   min_spacing='5x', wake_loss_multiplier=1, ga_kwargs=None,
-                   output_request=('system_capacity', 'cf_mean'),
-                   ws_bins=(0.0, 20.0, 5.0), wd_bins=(0.0, 360.0, 45.0),
-                   excl_dict=None, inclusion_mask=None,
-                   area_filter_kernel='queen', min_area=None,
-                   resolution=64, excl_area=0.0081, data_layers=None,
-                   gids=None, exclusion_shape=None, slice_lookup=None,
-                   prior_meta=None, gid_map=None, bias_correct=None,
-                   pre_loaded_data=None):
+    def run_serial(
+        cls,
+        excl_fpath,
+        res_fpath,
+        tm_dset,
+        sam_sys_inputs,
+        objective_function,
+        capital_cost_function,
+        fixed_operating_cost_function,
+        variable_operating_cost_function,
+        min_spacing="5x",
+        wake_loss_multiplier=1,
+        ga_kwargs=None,
+        output_request=("system_capacity", "cf_mean"),
+        ws_bins=(0.0, 20.0, 5.0),
+        wd_bins=(0.0, 360.0, 45.0),
+        excl_dict=None,
+        inclusion_mask=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        resolution=64,
+        excl_area=0.0081,
+        data_layers=None,
+        gids=None,
+        exclusion_shape=None,
+        slice_lookup=None,
+        prior_meta=None,
+        gid_map=None,
+        bias_correct=None,
+        pre_loaded_data=None,
+    ):
         """
         Standalone serial method to run bespoke optimization.
         See BespokeWindPlants docstring for parameter description.
 
         This method can only take a single sam_sys_inputs... For a spatially
         variant gid-to-config mapping, see the BespokeWindPlants class methods.
 
@@ -2191,26 +2418,27 @@
             if exclusion_shape is None:
                 exclusion_shape = sc.exclusions.shape
 
         cls._check_inclusion_mask(inclusion_mask, gids, exclusion_shape)
         Handler = BespokeSinglePlant.get_wind_handler(res_fpath)
 
         # pre-extract handlers so they are not repeatedly initialized
-        file_kwargs = {'excl_dict': excl_dict,
-                       'area_filter_kernel': area_filter_kernel,
-                       'min_area': min_area,
-                       'h5_handler': Handler,
-                       }
+        file_kwargs = {
+            "excl_dict": excl_dict,
+            "area_filter_kernel": area_filter_kernel,
+            "min_area": min_area,
+            "h5_handler": Handler,
+        }
 
         with AggFileHandler(excl_fpath, res_fpath, **file_kwargs) as fh:
             n_finished = 0
             for gid in gids:
                 gid_inclusions = cls._get_gid_inclusion_mask(
-                    inclusion_mask, gid, slice_lookup,
-                    resolution=resolution)
+                    inclusion_mask, gid, slice_lookup, resolution=resolution
+                )
                 try:
                     bsp_plant_out = BespokeSinglePlant.run(
                         gid,
                         fh.exclusions,
                         fh.h5,
                         tm_dset,
                         sam_sys_inputs,
@@ -2230,28 +2458,34 @@
                         excl_area=excl_area,
                         data_layers=data_layers,
                         exclusion_shape=exclusion_shape,
                         prior_meta=prior_meta,
                         gid_map=gid_map,
                         bias_correct=bias_correct,
                         pre_loaded_data=pre_loaded_data,
-                        close=False)
+                        close=False,
+                    )
 
                 except EmptySupplyCurvePointError:
-                    logger.debug('SC gid {} is fully excluded or does not '
-                                 'have any valid source data!'.format(gid))
+                    logger.debug(
+                        "SC gid {} is fully excluded or does not "
+                        "have any valid source data!".format(gid)
+                    )
                 except Exception as e:
-                    msg = 'SC gid {} failed!'.format(gid)
+                    msg = "SC gid {} failed!".format(gid)
                     logger.exception(msg)
                     raise RuntimeError(msg) from e
                 else:
                     n_finished += 1
-                    logger.debug('Serial bespoke: '
-                                 '{} out of {} points complete'
-                                 .format(n_finished, len(gids)))
+                    logger.debug(
+                        "Serial bespoke: "
+                        "{} out of {} points complete".format(
+                            n_finished, len(gids)
+                        )
+                    )
                     log_mem(logger)
                     out[gid] = bsp_plant_out
 
         return out
 
     def run_parallel(self, max_workers=None):
         """Run the bespoke optimization for many supply curve points in
@@ -2265,76 +2499,85 @@
 
         Returns
         -------
         out : dict
             Bespoke outputs keyed by sc point gid
         """
 
-        logger.info('Running bespoke optimization for points {} through {} '
-                    'at a resolution of {} on {} cores.'
-                    .format(self.gids[0], self.gids[-1], self._resolution,
-                            max_workers))
+        logger.info(
+            "Running bespoke optimization for points {} through {} "
+            "at a resolution of {} on {} cores.".format(
+                self.gids[0], self.gids[-1], self._resolution, max_workers
+            )
+        )
 
         futures = []
         out = {}
         n_finished = 0
-        loggers = [__name__, 'reV.supply_curve.point_summary', 'reV']
+        loggers = [__name__, "reV.supply_curve.point_summary", "reV"]
         with SpawnProcessPool(max_workers=max_workers, loggers=loggers) as exe:
-
             # iterate through split executions, submitting each to worker
             for gid in self.gids:
                 # submit executions and append to futures list
                 gid_incl_mask = None
                 if self._inclusion_mask is not None:
                     rs, cs = self.slice_lookup[gid]
                     gid_incl_mask = self._inclusion_mask[rs, cs]
 
-                futures.append(exe.submit(
-                    self.run_serial,
-                    self._excl_fpath,
-                    self._res_fpath,
-                    self._tm_dset,
-                    self.sam_sys_inputs_with_site_data(gid),
-                    self._obj_fun,
-                    self._cap_cost_fun,
-                    self._foc_fun,
-                    self._voc_fun,
-                    self._min_spacing,
-                    wake_loss_multiplier=self._wake_loss_multiplier,
-                    ga_kwargs=self._ga_kwargs,
-                    output_request=self._output_request,
-                    ws_bins=self._ws_bins,
-                    wd_bins=self._wd_bins,
-                    excl_dict=self._excl_dict,
-                    inclusion_mask=gid_incl_mask,
-                    area_filter_kernel=self._area_filter_kernel,
-                    min_area=self._min_area,
-                    resolution=self._resolution,
-                    excl_area=self._excl_area,
-                    data_layers=self._data_layers,
-                    gids=gid,
-                    exclusion_shape=self.shape,
-                    slice_lookup=copy.deepcopy(self.slice_lookup),
-                    prior_meta=self._get_prior_meta(gid),
-                    gid_map=self._gid_map,
-                    bias_correct=self._get_bc_for_gid(gid),
-                    pre_loaded_data=self._pre_loaded_data_for_sc_gid(gid)))
+                futures.append(
+                    exe.submit(
+                        self.run_serial,
+                        self._excl_fpath,
+                        self._res_fpath,
+                        self._tm_dset,
+                        self.sam_sys_inputs_with_site_data(gid),
+                        self._obj_fun,
+                        self._cap_cost_fun,
+                        self._foc_fun,
+                        self._voc_fun,
+                        self._min_spacing,
+                        wake_loss_multiplier=self._wake_loss_multiplier,
+                        ga_kwargs=self._ga_kwargs,
+                        output_request=self._output_request,
+                        ws_bins=self._ws_bins,
+                        wd_bins=self._wd_bins,
+                        excl_dict=self._excl_dict,
+                        inclusion_mask=gid_incl_mask,
+                        area_filter_kernel=self._area_filter_kernel,
+                        min_area=self._min_area,
+                        resolution=self._resolution,
+                        excl_area=self._excl_area,
+                        data_layers=self._data_layers,
+                        gids=gid,
+                        exclusion_shape=self.shape,
+                        slice_lookup=copy.deepcopy(self.slice_lookup),
+                        prior_meta=self._get_prior_meta(gid),
+                        gid_map=self._gid_map,
+                        bias_correct=self._get_bc_for_gid(gid),
+                        pre_loaded_data=self._pre_loaded_data_for_sc_gid(gid),
+                    )
+                )
 
             # gather results
             for future in as_completed(futures):
                 n_finished += 1
                 out.update(future.result())
                 if n_finished % 10 == 0:
                     mem = psutil.virtual_memory()
-                    logger.info('Parallel bespoke futures collected: '
-                                '{} out of {}. Memory usage is {:.3f} GB out '
-                                'of {:.3f} GB ({:.2f}% utilized).'
-                                .format(n_finished, len(futures),
-                                        mem.used / 1e9, mem.total / 1e9,
-                                        100 * mem.used / mem.total))
+                    logger.info(
+                        "Parallel bespoke futures collected: "
+                        "{} out of {}. Memory usage is {:.3f} GB out "
+                        "of {:.3f} GB ({:.2f}% utilized).".format(
+                            n_finished,
+                            len(futures),
+                            mem.used / 1e9,
+                            mem.total / 1e9,
+                            100 * mem.used / mem.total,
+                        )
+                    )
 
         return out
 
     def run(self, out_fpath=None, max_workers=None):
         """Run the bespoke wind plant optimization in serial or parallel.
 
         Parameters
@@ -2352,15 +2595,15 @@
         -------
         str | None
             Path to output HDF5 file, or ``None`` if results were not
             written to disk.
         """
 
         # parallel job distribution test.
-        if self._obj_fun == 'test':
+        if self._obj_fun == "test":
             return True
 
         if max_workers == 1:
             slice_lookup = copy.deepcopy(self.slice_lookup)
             for gid in self.gids:
                 gid_incl_mask = None
                 if self._inclusion_mask is not None:
@@ -2370,41 +2613,43 @@
                 sam_inputs = self.sam_sys_inputs_with_site_data(gid)
                 prior_meta = self._get_prior_meta(gid)
                 pre_loaded_data = self._pre_loaded_data_for_sc_gid(gid)
                 afk = self._area_filter_kernel
                 wlm = self._wake_loss_multiplier
                 i_bc = self._get_bc_for_gid(gid)
 
-                si = self.run_serial(self._excl_fpath,
-                                     self._res_fpath,
-                                     self._tm_dset,
-                                     sam_inputs,
-                                     self._obj_fun,
-                                     self._cap_cost_fun,
-                                     self._foc_fun,
-                                     self._voc_fun,
-                                     min_spacing=self._min_spacing,
-                                     wake_loss_multiplier=wlm,
-                                     ga_kwargs=self._ga_kwargs,
-                                     output_request=self._output_request,
-                                     ws_bins=self._ws_bins,
-                                     wd_bins=self._wd_bins,
-                                     excl_dict=self._excl_dict,
-                                     inclusion_mask=gid_incl_mask,
-                                     area_filter_kernel=afk,
-                                     min_area=self._min_area,
-                                     resolution=self._resolution,
-                                     excl_area=self._excl_area,
-                                     data_layers=self._data_layers,
-                                     slice_lookup=slice_lookup,
-                                     prior_meta=prior_meta,
-                                     gid_map=self._gid_map,
-                                     bias_correct=i_bc,
-                                     gids=gid,
-                                     pre_loaded_data=pre_loaded_data)
+                si = self.run_serial(
+                    self._excl_fpath,
+                    self._res_fpath,
+                    self._tm_dset,
+                    sam_inputs,
+                    self._obj_fun,
+                    self._cap_cost_fun,
+                    self._foc_fun,
+                    self._voc_fun,
+                    min_spacing=self._min_spacing,
+                    wake_loss_multiplier=wlm,
+                    ga_kwargs=self._ga_kwargs,
+                    output_request=self._output_request,
+                    ws_bins=self._ws_bins,
+                    wd_bins=self._wd_bins,
+                    excl_dict=self._excl_dict,
+                    inclusion_mask=gid_incl_mask,
+                    area_filter_kernel=afk,
+                    min_area=self._min_area,
+                    resolution=self._resolution,
+                    excl_area=self._excl_area,
+                    data_layers=self._data_layers,
+                    slice_lookup=slice_lookup,
+                    prior_meta=prior_meta,
+                    gid_map=self._gid_map,
+                    bias_correct=i_bc,
+                    gids=gid,
+                    pre_loaded_data=pre_loaded_data,
+                )
                 self._outputs.update(si)
         else:
             self._outputs = self.run_parallel(max_workers=max_workers)
 
         if out_fpath is not None:
             out_fpath = self.save_outputs(out_fpath)
```

### Comparing `NREL-reV-0.8.7/reV/bespoke/cli_bespoke.py` & `NREL-reV-0.8.9/reV/bespoke/cli_bespoke.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/bespoke/gradient_free.py` & `NREL-reV-0.8.9/reV/bespoke/gradient_free.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/bespoke/pack_turbs.py` & `NREL-reV-0.8.9/reV/bespoke/pack_turbs.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/bespoke/place_turbines.py` & `NREL-reV-0.8.9/reV/bespoke/place_turbines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=inconsistent-return-statements
 """
 place turbines for bespoke wind plants
 """
 import numpy as np
+from shapely.geometry import MultiPoint, MultiPolygon, Point, Polygon
 
-from shapely.geometry import Point, Polygon, MultiPolygon, MultiPoint
-
-from reV.bespoke.pack_turbs import PackTurbines
 from reV.bespoke.gradient_free import GeneticAlgorithm
+from reV.bespoke.pack_turbs import PackTurbines
 from reV.utilities.exceptions import WhileLoopPackingError
 
 
 def none_until_optimized(func):
     """Decorator that returns None until `PlaceTurbines` is optimized.
 
     Meant for exclusive use in `PlaceTurbines` and its subclasses.
@@ -186,15 +185,15 @@
                 self.packing_polygons = packing_polygons
             elif isinstance(packing_polygons, Polygon):
                 self.packing_polygons = MultiPolygon([packing_polygons])
             else:
                 self.packing_polygons = MultiPolygon([])
 
     def initialize_packing(self):
-        """run the turbine packing algorithm (maximizing plant capacity) to
+        """Run the turbine packing algorithm (maximizing plant capacity) to
         define potential turbine locations that will be used as design
         variables in the gentic algorithm.
         """
         packing = PackTurbines(self.min_spacing, self.packing_polygons)
         nturbs = 1E6
         mult = 1.0
         iters = 0
@@ -360,15 +359,15 @@
             'capital_cost_multiplier', 1) / system_capacity
         return eval(self.capital_cost_function, globals(), locals()) * mult
 
     @property
     def fixed_charge_rate(self):
         """Fixed charge rate if input to the SAM WindPowerPD object, None if
         not found in inputs."""
-        return self.wind_plant.sam_sys_inputs.get('fixed_charge_rate', None)
+        return self.wind_plant.sam_sys_inputs.get("fixed_charge_rate", None)
 
     @property
     @none_until_optimized
     def turbine_x(self):
         """This is the final optimized turbine x locations (m)"""
         return self.x_locations[self.optimized_design_variables]
 
@@ -391,15 +390,16 @@
         return self.turbine_capacity * self.nturbs
 
     @property
     @none_until_optimized
     def convex_hull(self):
         """This is the convex hull of the turbine locations"""
         turbines = MultiPoint([Point(x, y)
-                               for x,y in zip(self.turbine_x, self.turbine_y)])
+                               for x, y in zip(self.turbine_x,
+                                               self.turbine_y)])
         return turbines.convex_hull
 
     @property
     @none_until_optimized
     def area(self):
         """This is the area available for wind turbine placement (km^2)"""
         return self.full_polygons.area / 1e6
```

### Comparing `NREL-reV-0.8.7/reV/bespoke/plotting_functions.py` & `NREL-reV-0.8.9/reV/bespoke/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/cli.py` & `NREL-reV-0.8.9/reV/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/config/base_analysis_config.py` & `NREL-reV-0.8.9/reV/config/base_analysis_config.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/config/base_config.py` & `NREL-reV-0.8.9/reV/config/base_config.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/config/cli_project_points.py` & `NREL-reV-0.8.9/reV/config/cli_project_points.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/config/curtailment.py` & `NREL-reV-0.8.9/reV/config/curtailment.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/config/execution.py` & `NREL-reV-0.8.9/reV/config/execution.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/config/output_request.py` & `NREL-reV-0.8.9/reV/config/output_request.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/config/project_points.py` & `NREL-reV-0.8.9/reV/config/project_points.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # -*- coding: utf-8 -*-
 """
 reV Project Points Configuration
 """
+
 import copy
 import logging
-import numpy as np
 import os
-import pandas as pd
 from warnings import warn
 
+import numpy as np
+import pandas as pd
+from rex.multi_file_resource import MultiFileResource
+from rex.resource import Resource
+from rex.resource_extraction.resource_extraction import (
+    MultiFileResourceX,
+    ResourceX,
+)
+from rex.utilities import check_res_file, parse_table
+
 from reV.config.curtailment import Curtailment
 from reV.config.sam_config import SAMConfig
+from reV.utilities import SiteDataField, SupplyCurveField
 from reV.utilities.exceptions import ConfigError, ConfigWarning
 
-from rex.resource import Resource
-from rex.multi_file_resource import MultiFileResource
-from rex.resource_extraction.resource_extraction import (ResourceX,
-                                                         MultiFileResourceX)
-from rex.utilities import check_res_file, parse_table
-
 logger = logging.getLogger(__name__)
 
 
 class PointsControl:
     """Class to manage and split ProjectPoints."""
+
     def __init__(self, project_points, sites_per_split=100):
         """
         Parameters
         ----------
         project_points : reV.config.ProjectPoints
             ProjectPoints instance to be split between execution workers.
         sites_per_split : int
@@ -42,35 +47,43 @@
         self._iter_list = []
 
     def __iter__(self):
         """Initialize the iterator by pre-splitting into a list attribute."""
         last_site = 0
         ilim = len(self.project_points)
 
-        logger.debug('PointsControl iterator initializing with sites '
-                     '{} through {}'.format(self.project_points.sites[0],
-                                            self.project_points.sites[-1]))
+        logger.debug(
+            "PointsControl iterator initializing with sites "
+            "{} through {}".format(
+                self.project_points.sites[0], self.project_points.sites[-1]
+            )
+        )
 
         # pre-initialize all iter objects
         while True:
             i0 = last_site
             i1 = np.min([i0 + self.sites_per_split, ilim])
             if i0 == i1:
                 break
 
             last_site = i1
 
-            new = self.split(i0, i1, self.project_points,
-                             sites_per_split=self.sites_per_split)
+            new = self.split(
+                i0,
+                i1,
+                self.project_points,
+                sites_per_split=self.sites_per_split,
+            )
             new._split_range = [i0, i1]
             self._iter_list.append(new)
 
-        logger.debug('PointsControl stopped iteration at attempted '
-                     'index of {}. Length of iterator is: {}'
-                     .format(i1, len(self)))
+        logger.debug(
+            "PointsControl stopped iteration at attempted "
+            "index of {}. Length of iterator is: {}".format(i1, len(self))
+        )
         return self
 
     def __next__(self):
         """Iterate through and return next site resource data.
 
         Returns
         -------
@@ -81,25 +94,30 @@
         if self._i < self.N:
             # Get next PointsControl from the iter list
             next_pc = self._iter_list[self._i]
         else:
             # No more points controllers left in initialized list
             raise StopIteration
 
-        logger.debug('PointsControl passing site project points '
-                     'with indices {} to {} on iteration #{} '
-                     .format(next_pc.split_range[0],
-                             next_pc.split_range[1], self._i))
+        logger.debug(
+            "PointsControl passing site project points "
+            "with indices {} to {} on iteration #{} ".format(
+                next_pc.split_range[0], next_pc.split_range[1], self._i
+            )
+        )
         self._i += 1
         return next_pc
 
     def __repr__(self):
-        msg = ("{} with {} sites from gid {} through {}"
-               .format(self.__class__.__name__, len(self.project_points),
-                       self.sites[0], self.sites[-1]))
+        msg = "{} with {} sites from gid {} through {}".format(
+            self.__class__.__name__,
+            len(self.project_points),
+            self.sites[0],
+            self.sites[-1],
+        )
         return msg
 
     def __len__(self):
         """Len is the number of possible iterations aka splits."""
         return int(np.ceil(len(self.project_points) / self.sites_per_split))
 
     @property
@@ -206,16 +224,17 @@
     >>> config_id_site0, SAM_config_dict_site0 = pp[0]
     >>> site_list_or_slice = pp.sites
     >>> site_list_or_slice = pp.get_sites_from_config(config_id)
     >>> ProjectPoints_sub = pp.split(0, 10, project_points)
     >>> h_list = pp.h
     """
 
-    def __init__(self, points, sam_configs, tech=None, res_file=None,
-                 curtailment=None):
+    def __init__(
+        self, points, sam_configs, tech=None, res_file=None, curtailment=None
+    ):
         """
         Parameters
         ----------
         points : int | slice | list | tuple | str | pd.DataFrame | dict
             Slice specifying project points, string pointing to a project
             points csv, or a dataframe containing the effective csv contents.
             Can also be a single integer site value.
@@ -265,45 +284,48 @@
             Configuration ID (variable name) specified in the sam_generation
             config section.
         config : dict
             Actual SAM input values in a single level dictionary with variable
             names (keys) and values.
         """
 
-        site_bool = (self.df['gid'] == site)
+        site_bool = self.df[SiteDataField.GID] == site
         try:
-            config_id = self.df.loc[site_bool, 'config'].values[0]
+            config_id = self.df.loc[site_bool, SiteDataField.CONFIG].values[0]
         except (KeyError, IndexError) as ex:
-            msg = ('Site {} not found in this instance of '
-                   'ProjectPoints. Available sites include: {}'
-                   .format(site, self.sites))
+            msg = (
+                "Site {} not found in this instance of "
+                "ProjectPoints. Available sites include: {}".format(
+                    site, self.sites
+                )
+            )
             logger.exception(msg)
             raise KeyError(msg) from ex
 
         return config_id, copy.deepcopy(self.sam_inputs[config_id])
 
     def __repr__(self):
-        msg = ("{} with {} sites from gid {} through {}"
-               .format(self.__class__.__name__, len(self),
-                       self.sites[0], self.sites[-1]))
+        msg = "{} with {} sites from gid {} through {}".format(
+            self.__class__.__name__, len(self), self.sites[0], self.sites[-1]
+        )
         return msg
 
     def __len__(self):
         """Length of this object is the number of sites."""
         return len(self.sites)
 
     @property
     def df(self):
         """Get the project points dataframe property.
 
         Returns
         -------
         _df : pd.DataFrame
             Table of sites and corresponding SAM configuration IDs.
-            Has columns 'gid' and 'config'.
+            Has columns "gid" and 'config'.
         """
         return self._df
 
     @property
     def sam_config_ids(self):
         """Get the SAM configs dictionary property.
 
@@ -380,15 +402,15 @@
 
         Returns
         -------
         sites : list
             List of integer sites (resource file gids) belonging to this
             instance of ProjectPoints.
         """
-        return self.df['gid'].values.tolist()
+        return self.df[SiteDataField.GID].values.tolist()
 
     @property
     def sites_as_slice(self):
         """Get the sites in slice format.
 
         Returns
         -------
@@ -421,29 +443,29 @@
         Returns
         -------
         _tech : str
             SAM technology to analyze (pvwattsv7, windpower, tcsmoltensalt,
             solarwaterheat, troughphysicalheat, lineardirectsteam)
             The string should be lower-cased with spaces and _ removed.
         """
-        return 'windpower' if 'wind' in self._tech.lower() else self._tech
+        return "windpower" if "wind" in self._tech.lower() else self._tech
 
     @property
     def h(self):
         """Get the hub heights corresponding to the site list.
 
         Returns
         -------
         _h : list | NoneType
             Hub heights corresponding to each site, taken from the sam config
             for each site. This is None if the technology is not wind.
         """
-        h_var = 'wind_turbine_hub_ht'
+        h_var = "wind_turbine_hub_ht"
         if self._h is None:
-            if 'wind' in self.tech:
+            if "wind" in self.tech:
                 # wind technology, get a list of h values
                 self._h = [self[site][1][h_var] for site in self.sites]
 
         return self._h
 
     @property
     def d(self):
@@ -452,17 +474,17 @@
         Returns
         -------
         _d : list | NoneType
             Resource depths (m) corresponding to each site, taken from
             the sam config for each site. This is None if the technology
             is not geothermal.
         """
-        d_var = 'resource_depth'
+        d_var = "resource_depth"
         if self._d is None:
-            if 'geothermal' in self.tech:
+            if "geothermal" in self.tech:
                 if d_var in self.df:
                     self._d = list(self.df[d_var])
                 else:
                     self._d = [self[site][1][d_var] for site in self.sites]
 
         return self._d
 
@@ -481,29 +503,30 @@
     @staticmethod
     def _parse_csv(fname):
         """Import project points from .csv
 
         Parameters
         ----------
         fname : str
-            Project points .csv file (with path). Must have 'gid' and 'config'
-            column names.
+            Project points .csv file (with path). Must have 'gid' and
+            'config' column names.
 
         Returns
         -------
         df : pd.DataFrame
             DataFrame mapping sites (gids) to SAM technology (config)
         """
         fname = fname.strip()
-        if fname.endswith('.csv'):
+        if fname.endswith(".csv"):
             df = pd.read_csv(fname)
         else:
-            raise ValueError('Config project points file must be '
-                             '.csv, but received: {}'
-                             .format(fname))
+            raise ValueError(
+                "Config project points file must be "
+                ".csv, but received: {}".format(fname)
+            )
 
         return df
 
     @staticmethod
     def _parse_sites(points, res_file=None):
         """Parse project points from list or slice
 
@@ -518,46 +541,49 @@
             points slice stop is None.
 
         Returns
         -------
         df : pd.DataFrame
             DataFrame mapping sites (gids) to SAM technology (config)
         """
-        df = pd.DataFrame(columns=['gid', 'config'])
+        df = pd.DataFrame(columns=[SiteDataField.GID, SiteDataField.CONFIG])
         if isinstance(points, int):
             points = [points]
         if isinstance(points, (list, tuple, np.ndarray)):
             # explicit site list, set directly
             if any(isinstance(i, (list, tuple, np.ndarray)) for i in points):
                 msg = "Provided project points is not flat: {}!".format(points)
                 logger.error(msg)
                 raise RuntimeError(msg)
 
-            df['gid'] = points
+            df[SiteDataField.GID] = points
         elif isinstance(points, slice):
             stop = points.stop
             if stop is None:
                 if res_file is None:
-                    raise ValueError('Must supply a resource file if '
-                                     'points is a slice of type '
-                                     ' slice(*, None, *)')
+                    raise ValueError(
+                        "Must supply a resource file if "
+                        "points is a slice of type "
+                        " slice(*, None, *)"
+                    )
 
                 multi_h5_res, _ = check_res_file(res_file)
                 if multi_h5_res:
                     stop = MultiFileResource(res_file).shape[1]
                 else:
                     stop = Resource(res_file).shape[1]
 
-            df['gid'] = list(range(*points.indices(stop)))
+            df[SiteDataField.GID] = list(range(*points.indices(stop)))
         else:
-            raise TypeError('Project Points sites needs to be set as a list, '
-                            'tuple, or slice, but was set as: {}'
-                            .format(type(points)))
+            raise TypeError(
+                "Project Points sites needs to be set as a list, "
+                "tuple, or slice, but was set as: {}".format(type(points))
+            )
 
-        df['config'] = None
+        df[SiteDataField.CONFIG] = None
 
         return df
 
     @classmethod
     def _parse_points(cls, points, res_file=None):
         """Generate the project points df from inputs
 
@@ -581,33 +607,41 @@
         elif isinstance(points, dict):
             df = pd.DataFrame(points)
         elif isinstance(points, (int, slice, list, tuple, np.ndarray)):
             df = cls._parse_sites(points, res_file=res_file)
         elif isinstance(points, pd.DataFrame):
             df = points
         else:
-            raise ValueError('Cannot parse Project points data from {}'
-                             .format(type(points)))
-
-        if 'gid' not in df.columns:
-            raise KeyError('Project points data must contain "gid" column.')
+            raise ValueError(
+                "Cannot parse Project points data from {}".format(type(points))
+            )
+        df = df.rename(SupplyCurveField.map_to(SiteDataField), axis=1)
+        if SiteDataField.GID not in df.columns:
+            raise KeyError(
+                "Project points data must contain "
+                f"{SiteDataField.GID} column."
+            )
 
         # pylint: disable=no-member
-        if 'config' not in df.columns:
-            df = cls._parse_sites(points["gid"].values, res_file=res_file)
+        if SiteDataField.CONFIG not in df.columns:
+            df = cls._parse_sites(
+                df[SiteDataField.GID].values, res_file=res_file
+            )
 
-        gids = df['gid'].values
+        gids = df[SiteDataField.GID].values
         if not np.array_equal(np.sort(gids), gids):
-            msg = ('WARNING: points are not in sequential order and will be '
-                   'sorted! The original order is being preserved under '
-                   'column "points_order"')
+            msg = (
+                "WARNING: points are not in sequential order and will be "
+                "sorted! The original order is being preserved under "
+                'column "points_order"'
+            )
             logger.warning(msg)
             warn(msg)
-            df['points_order'] = df.index.values
-            df = df.sort_values('gid').reset_index(drop=True)
+            df["points_order"] = df.index.values
+            df = df.sort_values(SiteDataField.GID).reset_index(drop=True)
 
         return df
 
     @staticmethod
     def _parse_sam_config(sam_config):
         """
         Create SAM files dictionary.
@@ -624,24 +658,24 @@
         _sam_config_obj : reV.config.sam_config.SAMConfig
             SAM configuration object.
         """
 
         if isinstance(sam_config, SAMConfig):
             return sam_config
 
+        if isinstance(sam_config, dict):
+            config_dict = sam_config
+        elif isinstance(sam_config, str):
+            config_dict = {sam_config: sam_config}
         else:
-            if isinstance(sam_config, dict):
-                config_dict = sam_config
-            elif isinstance(sam_config, str):
-                config_dict = {sam_config: sam_config}
-            else:
-                raise ValueError('Cannot parse SAM configs from {}'
-                                 .format(type(sam_config)))
+            raise ValueError(
+                "Cannot parse SAM configs from {}".format(type(sam_config))
+            )
 
-            return SAMConfig(config_dict)
+        return SAMConfig(config_dict)
 
     @staticmethod
     def _parse_curtailment(curtailment_input):
         """Parse curtailment config object.
 
         Parameters
         ----------
@@ -666,18 +700,20 @@
 
         elif isinstance(curtailment_input, (Curtailment, type(None))):
             # pre-initialized curtailment object or no curtailment (None)
             curtailment = curtailment_input
 
         else:
             curtailment = None
-            warn('Curtailment inputs not recognized. Received curtailment '
-                 'input of type: "{}". Expected None, dict, str, or '
-                 'Curtailment object. Defaulting to no curtailment.',
-                 ConfigWarning)
+            warn(
+                "Curtailment inputs not recognized. Received curtailment "
+                'input of type: "{}". Expected None, dict, str, or '
+                "Curtailment object. Defaulting to no curtailment.",
+                ConfigWarning,
+            )
 
         return curtailment
 
     def index(self, gid):
         """Get the index location (iloc not loc) for a resource gid found in
         the project points.
 
@@ -687,71 +723,80 @@
             Resource GID found in the project points gid column.
 
         Returns
         -------
         ind : int
             Row index of gid in the project points dataframe.
         """
-        if gid not in self._df['gid'].values:
-            e = ('Requested resource gid {} is not present in the project '
-                 'points dataframe. Cannot return row index.'.format(gid))
+        if gid not in self._df[SiteDataField.GID].values:
+            e = (
+                "Requested resource gid {} is not present in the project "
+                "points dataframe. Cannot return row index.".format(gid)
+            )
             logger.error(e)
             raise ConfigError(e)
 
-        ind = np.where(self._df['gid'] == gid)[0][0]
+        ind = np.where(self._df[SiteDataField.GID] == gid)[0][0]
 
         return ind
 
     def _check_points_config_mapping(self):
         """
         Check to ensure the project points (df) and SAM configs
         (sam_config_obj) are compatible. Update as necessary or break
         """
         # Extract unique config refences from project_points DataFrame
-        df_configs = self.df['config'].unique()
+        df_configs = self.df[SiteDataField.CONFIG].unique()
         sam_configs = self.sam_inputs
 
         # Checks to make sure that the same number of SAM config files
         # as references in project_points DataFrame
         if len(df_configs) > len(sam_configs):
-            msg = ('Points references {} configs while only '
-                   '{} SAM configs were provided!'
-                   .format(len(df_configs), len(sam_configs)))
+            msg = (
+                "Points references {} configs while only "
+                "{} SAM configs were provided!".format(
+                    len(df_configs), len(sam_configs)
+                )
+            )
             logger.error(msg)
             raise ConfigError(msg)
 
         if len(df_configs) == 1 and df_configs[0] is None:
-            self._df['config'] = list(sam_configs)[0]
-            df_configs = self.df['config'].unique()
+            self._df[SiteDataField.CONFIG] = list(sam_configs)[0]
+            df_configs = self.df[SiteDataField.CONFIG].unique()
 
         # Check to see if config references in project_points DataFrame
         # are valid file paths, if compare with SAM configs
         # and update as needed
         configs = {}
         for config in df_configs:
             if os.path.isfile(config):
                 configs[config] = config
             elif config in sam_configs:
                 configs[config] = sam_configs[config]
             else:
-                msg = ('{} does not map to a valid configuration file'
-                       .format(config))
+                msg = "{} does not map to a valid configuration file".format(
+                    config
+                )
                 logger.error(msg)
                 raise ConfigError(msg)
 
         # If configs has any keys that are not in sam_configs then
         # something really weird happened so raise an error.
         if any(set(configs) - set(sam_configs)):
-            msg = ('A wild config has appeared! Requested config keys for '
-                   'ProjectPoints are {} and previous config keys are {}'
-                   .format(list(configs), list(sam_configs)))
+            msg = (
+                "A wild config has appeared! Requested config keys for "
+                "ProjectPoints are {} and previous config keys are {}".format(
+                    list(configs), list(sam_configs)
+                )
+            )
             logger.error(msg)
             raise ConfigError(msg)
 
-    def join_df(self, df2, key='gid'):
+    def join_df(self, df2, key=SiteDataField.GID):
         """Join new df2 to the _df attribute using the _df's gid as pkey.
 
         This can be used to add site-specific data to the project_points,
         taking advantage of the points_control iterator/split functions such
         that only the relevant site data is passed to the analysis functions.
 
         Parameters
@@ -763,16 +808,23 @@
         key : str
             Primary key of df2 to be joined to the _df attribute (this
             instance of the project points dataframe). Primary key
             of the self._df attribute is fixed as the gid column.
         """
         # ensure df2 doesnt have any duplicate columns for suffix reasons.
         df2_cols = [c for c in df2.columns if c not in self._df or c == key]
-        self._df = pd.merge(self._df, df2[df2_cols], how='left', left_on='gid',
-                            right_on=key, copy=False, validate='1:1')
+        self._df = pd.merge(
+            self._df,
+            df2[df2_cols],
+            how="left",
+            left_on=SiteDataField.GID,
+            right_on=key,
+            copy=False,
+            validate="1:1",
+        )
 
     def get_sites_from_config(self, config):
         """Get a site list that corresponds to a config key.
 
         Parameters
         ----------
         config : str
@@ -780,15 +832,17 @@
 
         Returns
         -------
         sites : list
             List of sites associated with the requested configuration ID. If
             the configuration ID is not recognized, an empty list is returned.
         """
-        sites = self.df.loc[(self.df['config'] == config), 'gid'].values
+        sites = self.df.loc[
+            (self.df[SiteDataField.CONFIG] == config), SiteDataField.GID
+        ].values
 
         return list(sites)
 
     @classmethod
     def split(cls, i0, i1, project_points):
         """Return split instance of a ProjectPoints instance w/ site subset.
 
@@ -813,56 +867,64 @@
             New instance of ProjectPoints with a subset of the following
             attributes: sites, project points df, and the self dictionary data
             struct.
         """
         # Extract DF subset with only index values between i0 and i1
         n = len(project_points)
         if i0 > n or i1 > n:
-            raise ValueError('{} and {} must be within the range of '
-                             'project_points (0 - {})'.format(i0, i1, n - 1))
+            raise ValueError(
+                "{} and {} must be within the range of "
+                "project_points (0 - {})".format(i0, i1, n - 1)
+            )
 
         points_df = project_points.df.iloc[i0:i1]
 
         # make a new instance of ProjectPoints with subset DF
-        sub = cls(points_df,
-                  project_points.sam_config_obj,
-                  project_points.tech,
-                  curtailment=project_points.curtailment)
+        sub = cls(
+            points_df,
+            project_points.sam_config_obj,
+            project_points.tech,
+            curtailment=project_points.curtailment,
+        )
 
         return sub
 
     @staticmethod
     def _parse_lat_lons(lat_lons):
-        msg = ('Expecting a pair or multiple pairs of latitude and '
-               'longitude coordinates!')
+        msg = (
+            "Expecting a pair or multiple pairs of latitude and "
+            "longitude coordinates!"
+        )
         if isinstance(lat_lons, str):
             lat_lons = parse_table(lat_lons)
-            cols = [c for c in lat_lons
-                    if c.lower().startswith(('lat', 'lon'))]
+            cols = [
+                c for c in lat_lons if c.lower().startswith(("lat", "lon"))
+            ]
             lat_lons = lat_lons[sorted(cols)].values
         elif isinstance(lat_lons, (list, tuple)):
             lat_lons = np.array(lat_lons)
         elif isinstance(lat_lons, (int, float)):
-            msg += ' Recieved a single coordinate value!'
+            msg += " Recieved a single coordinate value!"
             logger.error(msg)
             raise ValueError(msg)
 
         if len(lat_lons.shape) == 1:
             lat_lons = np.expand_dims(lat_lons, axis=0)
 
         if lat_lons.shape[1] != 2:
-            msg += ' Received {} coordinate values!'.format(lat_lons.shape[1])
+            msg += " Received {} coordinate values!".format(lat_lons.shape[1])
             logger.error(msg)
             raise ValueError(msg)
 
         return lat_lons
 
     @classmethod
-    def lat_lon_coords(cls, lat_lons, res_file, sam_configs, tech=None,
-                       curtailment=None):
+    def lat_lon_coords(
+        cls, lat_lons, res_file, sam_configs, tech=None, curtailment=None
+    ):
         """
         Generate ProjectPoints for gids nearest to given latitude longitudes
 
         Parameters
         ----------
         lat_lons : str | tuple | list | ndarray
             Pair or pairs of latitude longitude coordinates
@@ -899,57 +961,68 @@
 
         multi_h5_res, hsds = check_res_file(res_file)
         if multi_h5_res:
             res_cls = MultiFileResourceX
             res_kwargs = {}
         else:
             res_cls = ResourceX
-            res_kwargs = {'hsds': hsds}
+            res_kwargs = {"hsds": hsds}
 
-        logger.info('Converting latitude longitude coordinates into nearest '
-                    'ProjectPoints')
-        logger.debug('- (lat, lon) pairs:\n{}'.format(lat_lons))
+        logger.info(
+            "Converting latitude longitude coordinates into nearest "
+            "ProjectPoints"
+        )
+        logger.debug("- (lat, lon) pairs:\n{}".format(lat_lons))
         with res_cls(res_file, **res_kwargs) as f:
             gids = f.lat_lon_gid(lat_lons)  # pylint: disable=no-member
 
         if isinstance(gids, int):
             gids = [gids]
         else:
             if len(gids) != len(np.unique(gids)):
-                uniques, pos, counts = np.unique(gids, return_counts=True,
-                                                 return_inverse=True)
+                uniques, pos, counts = np.unique(
+                    gids, return_counts=True, return_inverse=True
+                )
                 duplicates = {}
                 for idx in np.where(counts > 1)[0]:
                     duplicate_lat_lons = lat_lons[np.where(pos == idx)[0]]
                     duplicates[uniques[idx]] = duplicate_lat_lons
 
-                msg = ('reV Cannot currently handle duplicate Resource gids! '
-                       'The given latitude and longitudes map to the same '
-                       'gids:\n{}'.format(duplicates))
+                msg = (
+                    "reV Cannot currently handle duplicate Resource gids! "
+                    "The given latitude and longitudes map to the same "
+                    "gids:\n{}".format(duplicates)
+                )
                 logger.error(msg)
                 raise RuntimeError(msg)
 
             gids = gids.tolist()
 
-        logger.debug('- Resource gids:\n{}'.format(gids))
+        logger.debug("- Resource gids:\n{}".format(gids))
 
-        pp = cls(gids, sam_configs, tech=tech, res_file=res_file,
-                 curtailment=curtailment)
+        pp = cls(
+            gids,
+            sam_configs,
+            tech=tech,
+            res_file=res_file,
+            curtailment=curtailment,
+        )
 
-        if 'points_order' in pp.df:
-            lat_lons = lat_lons[pp.df['points_order'].values]
+        if "points_order" in pp.df:
+            lat_lons = lat_lons[pp.df["points_order"].values]
 
-        pp._df['latitude'] = lat_lons[:, 0]
-        pp._df['longitude'] = lat_lons[:, 1]
+        pp._df["latitude"] = lat_lons[:, 0]
+        pp._df["longitude"] = lat_lons[:, 1]
 
         return pp
 
     @classmethod
-    def regions(cls, regions, res_file, sam_configs, tech=None,
-                curtailment=None):
+    def regions(
+        cls, regions, res_file, sam_configs, tech=None, curtailment=None
+    ):
         """
         Generate ProjectPoints for gids nearest to given latitude longitudes
 
         Parameters
         ----------
         regions : dict
             Dictionary of regions to extract points for in the form:
@@ -985,36 +1058,43 @@
         """
         multi_h5_res, hsds = check_res_file(res_file)
         if multi_h5_res:
             res_cls = MultiFileResourceX
         else:
             res_cls = ResourceX
 
-        logger.info('Extracting ProjectPoints for desired regions')
+        logger.info("Extracting ProjectPoints for desired regions")
         points = []
         with res_cls(res_file, hsds=hsds) as f:
             meta = f.meta
             for region, region_col in regions.items():
-                logger.debug('- {}: {}'.format(region_col, region))
+                logger.debug("- {}: {}".format(region_col, region))
                 # pylint: disable=no-member
                 gids = f.region_gids(region, region_col=region_col)
-                logger.debug('- Resource gids:\n{}'.format(gids))
+                logger.debug("- Resource gids:\n{}".format(gids))
                 if points:
                     duplicates = np.intersect1d(gids, points).tolist()
                     if duplicates:
-                        msg = ('reV Cannot currently handle duplicate '
-                               'Resource gids! The given regions containg the '
-                               'same gids:\n{}'.format(duplicates))
+                        msg = (
+                            "reV Cannot currently handle duplicate "
+                            "Resource gids! The given regions containg the "
+                            "same gids:\n{}".format(duplicates)
+                        )
                         logger.error(msg)
                         raise RuntimeError(msg)
 
                 points.extend(gids.tolist())
 
-        pp = cls(points, sam_configs, tech=tech, res_file=res_file,
-                 curtailment=curtailment)
+        pp = cls(
+            points,
+            sam_configs,
+            tech=tech,
+            res_file=res_file,
+            curtailment=curtailment,
+        )
 
         meta = meta.loc[pp.sites]
         cols = list(set(regions.values()))
         for c in cols:
             pp._df[c] = meta[c].values
 
         return pp
```

### Comparing `NREL-reV-0.8.7/reV/config/sam_config.py` & `NREL-reV-0.8.9/reV/config/sam_config.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/econ/cli_econ.py` & `NREL-reV-0.8.9/reV/econ/cli_econ.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/econ/econ.py` & `NREL-reV-0.8.9/reV/econ/econ.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 # -*- coding: utf-8 -*-
-"""
-reV econ module (lcoe-fcr, single owner, etc...)
-"""
+"""reV econ module (lcoe-fcr, single owner, etc...)"""
 import logging
-import numpy as np
 import os
-import pandas as pd
 import pprint
 from warnings import warn
 
+import numpy as np
+import pandas as pd
+from rex.multi_file_resource import MultiFileResource
+from rex.resource import Resource
+from rex.utilities.utilities import check_res_file
+
 from reV.config.project_points import PointsControl
 from reV.generation.base import BaseGen
 from reV.handlers.outputs import Outputs
 from reV.SAM.econ import LCOE as SAM_LCOE
 from reV.SAM.econ import SingleOwner
 from reV.SAM.windbos import WindBos
-from reV.utilities.exceptions import (ExecutionError, OffshoreWindInputWarning)
-from reV.utilities import ModuleName
-
-from rex.resource import Resource
-from rex.multi_file_resource import MultiFileResource
-from rex.utilities.utilities import check_res_file
+from reV.utilities import ModuleName, ResourceMetaField
+from reV.utilities.exceptions import ExecutionError, OffshoreWindInputWarning
 
 logger = logging.getLogger(__name__)
 
 
 class Econ(BaseGen):
     """Econ"""
 
     # Mapping of reV econ output strings to SAM econ modules
-    OPTIONS = {'lcoe_fcr': SAM_LCOE,
-               'ppa_price': SingleOwner,
-               'project_return_aftertax_npv': SingleOwner,
-               'lcoe_real': SingleOwner,
-               'lcoe_nom': SingleOwner,
-               'flip_actual_irr': SingleOwner,
-               'gross_revenue': SingleOwner,
-               'total_installed_cost': WindBos,
-               'turbine_cost': WindBos,
-               'sales_tax_cost': WindBos,
-               'bos_cost': WindBos,
-               'fixed_charge_rate': SAM_LCOE,
-               'capital_cost': SAM_LCOE,
-               'fixed_operating_cost': SAM_LCOE,
-               'variable_operating_cost': SAM_LCOE,
-               }
+    OPTIONS = {
+        "lcoe_fcr": SAM_LCOE,
+        "ppa_price": SingleOwner,
+        "project_return_aftertax_npv": SingleOwner,
+        "lcoe_real": SingleOwner,
+        "lcoe_nom": SingleOwner,
+        "flip_actual_irr": SingleOwner,
+        "gross_revenue": SingleOwner,
+        "total_installed_cost": WindBos,
+        "turbine_cost": WindBos,
+        "sales_tax_cost": WindBos,
+        "bos_cost": WindBos,
+        "fixed_charge_rate": SAM_LCOE,
+        "capital_cost": SAM_LCOE,
+        "fixed_operating_cost": SAM_LCOE,
+        "variable_operating_cost": SAM_LCOE,
+    }
     """Available ``reV`` econ `output_request` options"""
 
     # Mapping of reV econ outputs to scale factors and units.
     # Type is scalar or array and corresponds to the SAM single-site output
     OUT_ATTRS = BaseGen.ECON_ATTRS
 
     def __init__(self, project_points, sam_files, cf_file, site_data=None,
                  output_request=('lcoe_fcr',), sites_per_worker=100,
                  memory_utilization_limit=0.4, append=False):
-        """reV econ analysis class.
+        """ReV econ analysis class.
 
         ``reV`` econ analysis runs SAM econ calculations, typically to
         compute LCOE (using :py:class:`PySAM.Lcoefcr.Lcoefcr`), though
         :py:class:`PySAM.Singleowner.Singleowner` or
         :py:class:`PySAM.Windbos.Windbos` calculations can also be
         performed simply by requesting outputs from those computation
         modules. See the keys of
@@ -172,25 +171,34 @@
             disk. By default, ``0.4``.
         append : bool
             Option to append econ datasets to source `cf_file`.
             By default, ``False``.
         """
 
         # get a points control instance
-        pc = self.get_pc(points=project_points, points_range=None,
-                         sam_configs=sam_files, cf_file=cf_file,
-                         sites_per_worker=sites_per_worker, append=append)
-
-        super().__init__(pc, output_request, site_data=site_data,
-                         memory_utilization_limit=memory_utilization_limit)
+        pc = self.get_pc(
+            points=project_points,
+            points_range=None,
+            sam_configs=sam_files,
+            cf_file=cf_file,
+            sites_per_worker=sites_per_worker,
+            append=append,
+        )
+
+        super().__init__(
+            pc,
+            output_request,
+            site_data=site_data,
+            memory_utilization_limit=memory_utilization_limit,
+        )
 
         self._cf_file = cf_file
         self._append = append
-        self._run_attrs['cf_file'] = cf_file
-        self._run_attrs['sam_module'] = self._sam_module.MODULE
+        self._run_attrs["cf_file"] = cf_file
+        self._run_attrs["sam_module"] = self._sam_module.MODULE
 
     @property
     def cf_file(self):
         """Get the capacity factor output filename and path.
 
         Returns
         -------
@@ -208,36 +216,37 @@
         _meta : pd.DataFrame
             Meta data from capacity factor outputs file.
         """
         if self._meta is None and self.cf_file is not None:
             with Outputs(self.cf_file) as cfh:
                 # only take meta that belongs to this project's site list
                 self._meta = cfh.meta[
-                    cfh.meta['gid'].isin(self.points_control.sites)]
+                    cfh.meta[ResourceMetaField.GID].isin(
+                        self.points_control.sites)]
 
-            if 'offshore' in self._meta:
-                if self._meta['offshore'].sum() > 1:
-                    w = ('Found offshore sites in econ meta data. '
-                         'This functionality has been deprecated. '
-                         'Please run the reV offshore module to '
-                         'calculate offshore wind lcoe.')
-                    warn(w, OffshoreWindInputWarning)
-                    logger.warning(w)
+            if ("offshore" in self._meta and self._meta["offshore"].sum() > 1):
+                w = ('Found offshore sites in econ meta data. '
+                     'This functionality has been deprecated. '
+                     'Please run the reV offshore module to '
+                     'calculate offshore wind lcoe.')
+                warn(w, OffshoreWindInputWarning)
+                logger.warning(w)
 
         elif self._meta is None and self.cf_file is None:
-            self._meta = pd.DataFrame({'gid': self.points_control.sites})
+            self._meta = pd.DataFrame(
+                {ResourceMetaField.GID: self.points_control.sites})
 
         return self._meta
 
     @property
     def time_index(self):
         """Get the generation resource time index data."""
         if self._time_index is None and self.cf_file is not None:
             with Outputs(self.cf_file) as cfh:
-                if 'time_index' in cfh.datasets:
+                if "time_index" in cfh.datasets:
                     self._time_index = cfh.time_index
 
         return self._time_index
 
     @staticmethod
     def _econ_append_pc(pp, cf_file, sites_per_worker=None):
         """
@@ -260,29 +269,36 @@
         """
         multi_h5_res, hsds = check_res_file(cf_file)
         if multi_h5_res:
             res_cls = MultiFileResource
             res_kwargs = {}
         else:
             res_cls = Resource
-            res_kwargs = {'hsds': hsds}
+            res_kwargs = {"hsds": hsds}
 
         with res_cls(cf_file, **res_kwargs) as f:
-            gid0 = f.meta['gid'].values[0]
-            gid1 = f.meta['gid'].values[-1]
+            gid0 = f.meta[ResourceMetaField.GID].values[0]
+            gid1 = f.meta[ResourceMetaField.GID].values[-1]
 
         i0 = pp.index(gid0)
         i1 = pp.index(gid1) + 1
         pc = PointsControl.split(i0, i1, pp, sites_per_split=sites_per_worker)
 
         return pc
 
     @classmethod
-    def get_pc(cls, points, points_range, sam_configs, cf_file,
-               sites_per_worker=None, append=False):
+    def get_pc(
+        cls,
+        points,
+        points_range,
+        sam_configs,
+        cf_file,
+        sites_per_worker=None,
+        append=False,
+    ):
         """
         Get a PointsControl instance.
 
         Parameters
         ----------
         points : slice | list | str | reV.config.project_points.PointsControl
             Slice specifying project points, or string pointing to a project
@@ -307,36 +323,43 @@
             over the out_fpath input.
 
         Returns
         -------
         pc : reV.config.project_points.PointsControl
             PointsControl object instance.
         """
-        pc = super().get_pc(points, points_range, sam_configs, ModuleName.ECON,
-                            sites_per_worker=sites_per_worker,
-                            res_file=cf_file)
+        pc = super().get_pc(
+            points,
+            points_range,
+            sam_configs,
+            ModuleName.ECON,
+            sites_per_worker=sites_per_worker,
+            res_file=cf_file,
+        )
 
         if append:
-            pc = cls._econ_append_pc(pc.project_points, cf_file,
-                                     sites_per_worker=sites_per_worker)
+            pc = cls._econ_append_pc(
+                pc.project_points, cf_file, sites_per_worker=sites_per_worker
+            )
 
         return pc
 
     @staticmethod
     def _run_single_worker(pc, econ_fun, output_request, **kwargs):
         """Run the SAM econ calculation.
 
         Parameters
         ----------
         pc : reV.config.project_points.PointsControl
             Iterable points control object from reV config module.
             Must have project_points with df property with all relevant
-            site-specific inputs and a 'gid' column. By passing site-specific
-            inputs in this dataframe, which was split using points_control,
-            only the data relevant to the current sites is passed.
+            site-specific inputs and a `SupplyCurveField.GID` column.
+            By passing site-specific inputs in this dataframe, which
+            was split using points_control, only the data relevant to
+            the current sites is passed.
         econ_fun : method
             reV_run() method from one of the econ modules (SingleOwner,
             SAM_LCOE, WindBos).
         output_request : str | list | tuple
             Economic output variable(s) requested from SAM.
         kwargs : dict
             Additional input parameters for the SAM run module.
@@ -350,23 +373,24 @@
 
         # make sure output request is a list
         if isinstance(output_request, str):
             output_request = [output_request]
 
         # Extract the site df from the project points df.
         site_df = pc.project_points.df
-        site_df = site_df.set_index('gid', drop=True)
+        site_df = site_df.set_index(ResourceMetaField.GID, drop=True)
 
         # SAM execute econ analysis based on output request
         try:
-            out = econ_fun(pc, site_df, output_request=output_request,
-                           **kwargs)
+            out = econ_fun(
+                pc, site_df, output_request=output_request, **kwargs
+            )
         except Exception as e:
             out = {}
-            logger.exception('Worker failed for PC: {}'.format(pc))
+            logger.exception("Worker failed for PC: {}".format(pc))
             raise e
 
         return out
 
     def _parse_output_request(self, req):
         """Set the output variables requested from generation.
 
@@ -381,45 +405,50 @@
             Output variables requested from SAM.
         """
 
         output_request = self._output_request_type_check(req)
 
         for request in output_request:
             if request not in self.OUT_ATTRS:
-                msg = ('User output request "{}" not recognized. '
-                       'Will attempt to extract from PySAM.'.format(request))
+                msg = (
+                    'User output request "{}" not recognized. '
+                    "Will attempt to extract from PySAM.".format(request)
+                )
                 logger.debug(msg)
 
-        modules = []
-        for request in output_request:
-            if request in self.OPTIONS:
-                modules.append(self.OPTIONS[request])
+        modules = [self.OPTIONS[request] for request in output_request
+                   if request in self.OPTIONS]
 
         if not any(modules):
-            msg = ('None of the user output requests were recognized. '
-                   'Cannot run reV econ. '
-                   'At least one of the following must be requested: {}'
-                   .format(list(self.OPTIONS.keys())))
+            msg = (
+                "None of the user output requests were recognized. "
+                "Cannot run reV econ. "
+                "At least one of the following must be requested: {}".format(
+                    list(self.OPTIONS.keys())
+                )
+            )
             logger.exception(msg)
             raise ExecutionError(msg)
 
         b1 = [m == modules[0] for m in modules]
         b2 = np.array([m == WindBos for m in modules])
         b3 = np.array([m == SingleOwner for m in modules])
 
         if all(b1):
             self._sam_module = modules[0]
             self._fun = modules[0].reV_run
         elif all(b2 | b3):
             self._sam_module = SingleOwner
             self._fun = SingleOwner.reV_run
         else:
-            msg = ('Econ outputs requested from different SAM modules not '
-                   'currently supported. Output request variables require '
-                   'SAM methods: {}'.format(modules))
+            msg = (
+                "Econ outputs requested from different SAM modules not "
+                "currently supported. Output request variables require "
+                "SAM methods: {}".format(modules)
+            )
             raise ValueError(msg)
 
         return list(set(output_request))
 
     def _get_data_shape(self, dset, n_sites):
         """Get the output array shape based on OUT_ATTRS or PySAM.Outputs.
 
@@ -437,30 +466,31 @@
         Returns
         -------
         shape : tuple
             1D or 2D shape tuple for dset.
         """
 
         if dset in self.site_data:
-            data_shape = (n_sites, )
+            data_shape = (n_sites,)
             data = self.site_data[dset].values[0]
 
             if isinstance(data, (list, tuple, np.ndarray, str)):
-                msg = ('Cannot pass through non-scalar site_data '
-                       'input key "{}" as an output_request!'.format(dset))
+                msg = (
+                    "Cannot pass through non-scalar site_data "
+                    'input key "{}" as an output_request!'.format(dset)
+                )
                 logger.error(msg)
                 raise ExecutionError(msg)
 
         else:
             data_shape = super()._get_data_shape(dset, n_sites)
 
         return data_shape
 
-    def run(self, out_fpath=None, max_workers=1, timeout=1800,
-            pool_size=None):
+    def run(self, out_fpath=None, max_workers=1, timeout=1800, pool_size=None):
         """Execute a parallel reV econ run with smart data flushing.
 
         Parameters
         ----------
         out_fpath : str, optional
             Path to output file. If this class was initialized with
             ``append=True``, this input has no effect. If ``None``, no
@@ -490,56 +520,78 @@
 
         # initialize output file or append econ data to gen file
         if self._append:
             self._out_fpath = self._cf_file
         else:
             self._init_fpath(out_fpath, ModuleName.ECON)
 
-        self._init_h5(mode='a' if self._append else 'w')
+        self._init_h5(mode="a" if self._append else "w")
         self._init_out_arrays()
 
         diff = list(set(self.points_control.sites)
-                    - set(self.meta['gid'].values))
+                    - set(self.meta[ResourceMetaField.GID].values))
         if diff:
-            raise Exception('The following analysis sites were requested '
-                            'through project points for econ but are not '
-                            'found in the CF file ("{}"): {}'
-                            .format(self.cf_file, diff))
+            raise Exception(
+                "The following analysis sites were requested "
+                "through project points for econ but are not "
+                'found in the CF file ("{}"): {}'.format(self.cf_file, diff)
+            )
 
         # make a kwarg dict
-        kwargs = {'output_request': self.output_request,
-                  'cf_file': self.cf_file,
-                  'year': self.year}
-
-        logger.info('Running econ with smart data flushing '
-                    'for: {}'.format(self.points_control))
-        logger.debug('The following project points were specified: "{}"'
-                     .format(self.project_points))
-        logger.debug('The following SAM configs are available to this run:\n{}'
-                     .format(pprint.pformat(self.sam_configs, indent=4)))
-        logger.debug('The SAM output variables have been requested:\n{}'
-                     .format(self.output_request))
+        kwargs = {
+            "output_request": self.output_request,
+            "cf_file": self.cf_file,
+            "year": self.year,
+        }
+
+        logger.info(
+            "Running econ with smart data flushing " "for: {}".format(
+                self.points_control
+            )
+        )
+        logger.debug(
+            'The following project points were specified: "{}"'.format(
+                self.project_points
+            )
+        )
+        logger.debug(
+            "The following SAM configs are available to this run:\n{}".format(
+                pprint.pformat(self.sam_configs, indent=4)
+            )
+        )
+        logger.debug(
+            "The SAM output variables have been requested:\n{}".format(
+                self.output_request
+            )
+        )
 
         try:
-            kwargs['econ_fun'] = self._fun
+            kwargs["econ_fun"] = self._fun
             if max_workers == 1:
-                logger.debug('Running serial econ for: {}'
-                             .format(self.points_control))
+                logger.debug(
+                    "Running serial econ for: {}".format(self.points_control)
+                )
                 for i, pc_sub in enumerate(self.points_control):
                     self.out = self._run_single_worker(pc_sub, **kwargs)
-                    logger.info('Finished reV econ serial compute for: {} '
-                                '(iteration {} out of {})'
-                                .format(pc_sub, i + 1,
-                                        len(self.points_control)))
+                    logger.info(
+                        "Finished reV econ serial compute for: {} "
+                        "(iteration {} out of {})".format(
+                            pc_sub, i + 1, len(self.points_control)
+                        )
+                    )
                 self.flush()
             else:
-                logger.debug('Running parallel econ for: {}'
-                             .format(self.points_control))
-                self._parallel_run(max_workers=max_workers,
-                                   pool_size=pool_size, timeout=timeout,
-                                   **kwargs)
+                logger.debug(
+                    "Running parallel econ for: {}".format(self.points_control)
+                )
+                self._parallel_run(
+                    max_workers=max_workers,
+                    pool_size=pool_size,
+                    timeout=timeout,
+                    **kwargs,
+                )
 
         except Exception as e:
-            logger.exception('SmartParallelJob.execute() failed for econ.')
+            logger.exception("SmartParallelJob.execute() failed for econ.")
             raise e
 
         return self._out_fpath
```

### Comparing `NREL-reV-0.8.7/reV/econ/economies_of_scale.py` & `NREL-reV-0.8.9/reV/econ/economies_of_scale.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # -*- coding: utf-8 -*-
 """
 reV module for calculating economies of scale where larger power plants will
 have reduced capital cost.
 """
-import logging
+
 import copy
+import logging
 import re
-import numpy as np  # pylint: disable=unused-import
+
+# pylint: disable=unused-import
+import numpy as np
 import pandas as pd
+from rex.utilities.utilities import check_eval_str
 
 from reV.econ.utilities import lcoe_fcr
-from rex.utilities.utilities import check_eval_str
+from reV.utilities import SupplyCurveField
 
 logger = logging.getLogger(__name__)
 
 
 class EconomiesOfScale:
     """Class to calculate economies of scale where power plant capital cost is
     reduced for larger power plants.
@@ -53,31 +57,34 @@
     def _preflight(self):
         """Run checks to validate EconomiesOfScale equation and input data."""
 
         if self._eqn is not None:
             check_eval_str(str(self._eqn))
 
         if isinstance(self._data, pd.DataFrame):
-            self._data = {k: self._data[k].values.flatten()
-                          for k in self._data.columns}
+            self._data = {
+                k: self._data[k].values.flatten() for k in self._data.columns
+            }
 
         if not isinstance(self._data, dict):
-            e = ('Cannot evaluate EconomiesOfScale with data input of type: {}'
-                 .format(type(self._data)))
+            e = (
+                "Cannot evaluate EconomiesOfScale with data input of type: "
+                "{}".format(type(self._data))
+            )
+
             logger.error(e)
             raise TypeError(e)
 
-        missing = []
-        for name in self.vars:
-            if name not in self._data:
-                missing.append(name)
+        missing = [name for name in self.vars if name not in self._data]
 
         if any(missing):
-            e = ('Cannot evaluate EconomiesOfScale, missing data for variables'
-                 ': {} for equation: {}'.format(missing, self._eqn))
+            e = (
+                "Cannot evaluate EconomiesOfScale, missing data for variables"
+                ": {} for equation: {}".format(missing, self._eqn)
+            )
             logger.error(e)
             raise KeyError(e)
 
     @staticmethod
     def is_num(s):
         """Check if a string is a number"""
         try:
@@ -86,15 +93,15 @@
             return False
         else:
             return True
 
     @staticmethod
     def is_method(s):
         """Check if a string is a numpy/pandas or python builtin method"""
-        return bool(s.startswith(('np.', 'pd.')) or s in dir(__builtins__))
+        return bool(s.startswith(("np.", "pd.")) or s in dir(__builtins__))
 
     @property
     def vars(self):
         """Get a list of variable names that the EconomiesOfScale equation
         uses as input.
 
         Returns
@@ -102,22 +109,21 @@
         vars : list
             List of strings representing variable names that were parsed from
             the equation string. This will return an empty list if the equation
             has no variables.
         """
         var_names = []
         if self._eqn is not None:
-            delimiters = ('*', '/', '+', '-', ' ', '(', ')', '[', ']', ',')
-            regex_pattern = '|'.join(map(re.escape, delimiters))
+            delimiters = ("*", "/", "+", "-", " ", "(", ")", "[", "]", ",")
+            regex_pattern = "|".join(map(re.escape, delimiters))
             var_names = []
             for sub in re.split(regex_pattern, str(self._eqn)):
-                if sub:
-                    if not self.is_num(sub) and not self.is_method(sub):
-                        var_names.append(sub)
-            var_names = sorted(list(set(var_names)))
+                if sub and not self.is_num(sub) and not self.is_method(sub):
+                    var_names.append(sub)
+            var_names = sorted(set(var_names))
 
         return var_names
 
     def _evaluate(self):
         """Evaluate the EconomiesOfScale equation with Independent variables
         parsed into a kwargs dictionary input.
 
@@ -158,17 +164,18 @@
         out = None
         for key in key_list:
             if key in input_dict:
                 out = input_dict[key]
                 break
 
         if out is None:
-            e = ('Could not find requested key list ({}) in the input '
-                 'dictionary keys: {}'
-                 .format(key_list, list(input_dict.keys())))
+            e = (
+                "Could not find requested key list ({}) in the input "
+                "dictionary keys: {}".format(key_list, list(input_dict.keys()))
+            )
             logger.error(e)
             raise KeyError(e)
 
         return out
 
     @property
     def capital_cost_scalar(self):
@@ -188,15 +195,18 @@
         """Unscaled (raw) capital cost found in the data input arg.
 
         Returns
         -------
         out : float | np.ndarray
             Unscaled (raw) capital_cost found in the data input arg.
         """
-        key_list = ['capital_cost', 'mean_capital_cost']
+        key_list = [
+            SupplyCurveField.CAPITAL_COST,
+            "mean_capital_cost",
+        ]
         return self._get_prioritized_keys(self._data, key_list)
 
     @property
     def scaled_capital_cost(self):
         """Capital cost found in the data input arg scaled by the evaluated
         EconomiesOfScale input equation.
 
@@ -215,54 +225,66 @@
         """Get the system capacity in kW (SAM input, not the reV supply
         curve capacity).
 
         Returns
         -------
         out : float | np.ndarray
         """
-        key_list = ['system_capacity', 'mean_system_capacity']
+        key_list = ["system_capacity", "mean_system_capacity"]
         return self._get_prioritized_keys(self._data, key_list)
 
     @property
     def fcr(self):
         """Fixed charge rate from input data arg
 
         Returns
         -------
         out : float | np.ndarray
             Fixed charge rate from input data arg
         """
-        key_list = ['fixed_charge_rate', 'mean_fixed_charge_rate',
-                    'fcr', 'mean_fcr']
+        key_list = [
+            SupplyCurveField.FIXED_CHARGE_RATE,
+            "mean_fixed_charge_rate",
+            "fcr",
+            "mean_fcr",
+        ]
         return self._get_prioritized_keys(self._data, key_list)
 
     @property
     def foc(self):
         """Fixed operating cost from input data arg
 
         Returns
         -------
         out : float | np.ndarray
             Fixed operating cost from input data arg
         """
-        key_list = ['fixed_operating_cost', 'mean_fixed_operating_cost',
-                    'foc', 'mean_foc']
+        key_list = [
+            SupplyCurveField.FIXED_OPERATING_COST,
+            "mean_fixed_operating_cost",
+            "foc",
+            "mean_foc",
+        ]
         return self._get_prioritized_keys(self._data, key_list)
 
     @property
     def voc(self):
         """Variable operating cost from input data arg
 
         Returns
         -------
         out : float | np.ndarray
             Variable operating cost from input data arg
         """
-        key_list = ['variable_operating_cost', 'mean_variable_operating_cost',
-                    'voc', 'mean_voc']
+        key_list = [
+            SupplyCurveField.VARIABLE_OPERATING_COST,
+            "mean_variable_operating_cost",
+            "voc",
+            "mean_voc",
+        ]
         return self._get_prioritized_keys(self._data, key_list)
 
     @property
     def aep(self):
         """Annual energy production back-calculated from the raw LCOE:
 
         AEP = (fcr * raw_cap_cost + foc) / raw_lcoe
@@ -280,15 +302,15 @@
     def raw_lcoe(self):
         """Raw LCOE taken from the input data
 
         Returns
         -------
         lcoe : float | np.ndarray
         """
-        key_list = ['raw_lcoe', 'mean_lcoe']
+        key_list = [SupplyCurveField.RAW_LCOE, SupplyCurveField.MEAN_LCOE]
         return copy.deepcopy(self._get_prioritized_keys(self._data, key_list))
 
     @property
     def scaled_lcoe(self):
         """LCOE calculated with the scaled capital cost based on the
         EconomiesOfScale input equation.
 
@@ -296,9 +318,10 @@
 
         Returns
         -------
         lcoe : float | np.ndarray
             LCOE calculated with the scaled capital cost based on the
             EconomiesOfScale input equation.
         """
-        return lcoe_fcr(self.fcr, self.scaled_capital_cost, self.foc,
-                        self.aep, self.voc)
+        return lcoe_fcr(
+            self.fcr, self.scaled_capital_cost, self.foc, self.aep, self.voc
+        )
```

### Comparing `NREL-reV-0.8.7/reV/econ/utilities.py` & `NREL-reV-0.8.9/reV/econ/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/generation/base.py` & `NREL-reV-0.8.9/reV/generation/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 # -*- coding: utf-8 -*-
 """
 reV base gen and econ module.
 """
-from abc import ABC, abstractmethod
 import copy
-from concurrent.futures import TimeoutError
+import json
 import logging
-import pandas as pd
-import numpy as np
 import os
-import psutil
-import json
 import sys
+from abc import ABC, abstractmethod
+from concurrent.futures import TimeoutError
 from warnings import warn
 
+import numpy as np
+import pandas as pd
+import psutil
+from rex.resource import Resource
+from rex.utilities.execution import SpawnProcessPool
+
 from reV.config.output_request import SAMOutputRequest
-from reV.config.project_points import ProjectPoints, PointsControl
+from reV.config.project_points import PointsControl, ProjectPoints
 from reV.handlers.outputs import Outputs
 from reV.SAM.version_checker import PySamVersionChecker
-from reV.utilities.exceptions import (OutputWarning, ExecutionError,
-                                      ParallelExecutionWarning,
-                                      OffshoreWindInputWarning)
-from reV.utilities import log_versions, ModuleName
-
-from rex.resource import Resource
-from rex.utilities.execution import SpawnProcessPool
+from reV.utilities import ModuleName, ResourceMetaField, log_versions
+from reV.utilities.exceptions import (
+    ExecutionError,
+    OffshoreWindInputWarning,
+    OutputWarning,
+    ParallelExecutionWarning,
+)
 
 logger = logging.getLogger(__name__)
 
 
 ATTR_DIR = os.path.dirname(os.path.realpath(__file__))
 ATTR_DIR = os.path.join(ATTR_DIR, 'output_attributes')
-with open(os.path.join(ATTR_DIR, 'other.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, 'other.json')) as f:
     OTHER_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'lcoe_fcr.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, 'lcoe_fcr.json')) as f:
     LCOE_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'single_owner.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, 'single_owner.json')) as f:
     SO_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'windbos.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, 'windbos.json')) as f:
     BOS_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'lcoe_fcr_inputs.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, 'lcoe_fcr_inputs.json')) as f:
     LCOE_IN_ATTRS = json.load(f)
 
 
 class BaseGen(ABC):
     """Base class for reV gen and econ classes to run SAM simulations."""
 
     # Mapping of reV requests to SAM objects that should be used for simulation
@@ -61,20 +64,27 @@
     ECON_ATTRS.update(SO_ATTRS)
     ECON_ATTRS.update(BOS_ATTRS)
     ECON_ATTRS.update(LCOE_IN_ATTRS)
 
     # SAM argument names used to calculate LCOE
     # Note that system_capacity is not included here because it is never used
     # downstream and could be confused with the supply_curve point capacity
-    LCOE_ARGS = ('fixed_charge_rate', 'capital_cost', 'fixed_operating_cost',
+    LCOE_ARGS = ('fixed_charge_rate', 'capital_cost',
+                 'fixed_operating_cost',
                  'variable_operating_cost')
 
-    def __init__(self, points_control, output_request, site_data=None,
-                 drop_leap=False, memory_utilization_limit=0.4,
-                 scale_outputs=True):
+    def __init__(
+        self,
+        points_control,
+        output_request,
+        site_data=None,
+        drop_leap=False,
+        memory_utilization_limit=0.4,
+        scale_outputs=True,
+    ):
         """
         Parameters
         ----------
         points_control : reV.config.project_points.PointsControl
             Project points control instance for site and SAM config spec.
         output_request : list | tuple
             Output variables requested from SAM.
@@ -102,19 +112,21 @@
         self._time_index = None
         self._sam_module = None
         self._sam_obj_default = None
         self._drop_leap = drop_leap
         self.mem_util_lim = memory_utilization_limit
         self.scale_outputs = scale_outputs
 
-        self._run_attrs = {'points_control': str(points_control),
-                           'output_request': output_request,
-                           'site_data': str(site_data),
-                           'drop_leap': str(drop_leap),
-                           'memory_utilization_limit': self.mem_util_lim}
+        self._run_attrs = {
+            "points_control": str(points_control),
+            "output_request": output_request,
+            "site_data": str(site_data),
+            "drop_leap": str(drop_leap),
+            "memory_utilization_limit": self.mem_util_lim,
+        }
 
         self._site_data = self._parse_site_data(site_data)
         self.add_site_data_to_pp(self._site_data)
         output_request = SAMOutputRequest(output_request)
         self._output_request = self._parse_output_request(output_request)
 
         # pre-initialize output arrays to store results when available.
@@ -170,19 +182,24 @@
             without violating memory limits.
         """
 
         if self._site_limit is None:
             tot_mem = psutil.virtual_memory().total / 1e6
             avail_mem = self.mem_util_lim * tot_mem
             self._site_limit = int(np.floor(avail_mem / self.site_mem))
-            logger.info('Limited to storing {0} sites in memory '
-                        '({1:.1f} GB total hardware, {2:.1f} GB available '
-                        'with {3:.1f}% utilization).'
-                        .format(self._site_limit, tot_mem / 1e3,
-                                avail_mem / 1e3, self.mem_util_lim * 100))
+            logger.info(
+                "Limited to storing {0} sites in memory "
+                "({1:.1f} GB total hardware, {2:.1f} GB available "
+                "with {3:.1f}% utilization).".format(
+                    self._site_limit,
+                    tot_mem / 1e3,
+                    avail_mem / 1e3,
+                    self.mem_util_lim * 100,
+                )
+            )
 
         return self._site_limit
 
     @property
     def site_mem(self):
         """Get the memory (MB) required to store all results for a single site.
 
@@ -195,25 +212,26 @@
 
         if self._site_mem is None:
             # average the memory usage over n sites
             # (for better understanding of array overhead)
             n = 100
             self._site_mem = 0
             for request in self.output_request:
-                dtype = 'float32'
+                dtype = "float32"
                 if request in self.OUT_ATTRS:
-                    dtype = self.OUT_ATTRS[request].get('dtype', 'float32')
+                    dtype = self.OUT_ATTRS[request].get("dtype", "float32")
 
                 shape = self._get_data_shape(request, n)
                 self._site_mem += sys.getsizeof(np.ones(shape, dtype=dtype))
 
             self._site_mem = self._site_mem / 1e6 / n
-            logger.info('Output results from a single site are calculated to '
-                        'use {0:.1f} KB of memory.'
-                        .format(self._site_mem / 1000))
+            logger.info(
+                "Output results from a single site are calculated to "
+                "use {0:.1f} KB of memory.".format(self._site_mem / 1000)
+            )
 
         return self._site_mem
 
     @property
     def points_control(self):
         """Get project points controller.
 
@@ -255,15 +273,15 @@
         -------
         sam_metas : dict
             Nested dictionary of SAM configuration files with module used
             at runtime
         """
         sam_metas = self.sam_configs.copy()
         for v in sam_metas.values():
-            v.update({'module': self._sam_module.MODULE})
+            v.update({"module": self._sam_module.MODULE})
 
         return sam_metas
 
     @property
     def sam_module(self):
         """Get the SAM module class to be used for SAM simulations.
 
@@ -280,15 +298,16 @@
 
         Returns
         -------
         meta : pd.DataFrame
             Meta data df for sites in project points. Column names are meta
             data variables, rows are different sites. The row index
             does not indicate the site number if the project points are
-            non-sequential or do not start from 0, so a 'gid' column is added.
+            non-sequential or do not start from 0, so a `SupplyCurveField.GID`
+            column is added.
         """
         return self._meta
 
     @property
     def time_index(self):
         """Get the resource time index data.
 
@@ -347,20 +366,20 @@
         -------
         out : dict
             Dictionary of gen or econ results from SAM.
         """
         out = {}
         for k, v in self._out.items():
             if k in self.OUT_ATTRS:
-                scale_factor = self.OUT_ATTRS[k].get('scale_factor', 1)
+                scale_factor = self.OUT_ATTRS[k].get("scale_factor", 1)
             else:
                 scale_factor = 1
 
             if scale_factor != 1 and self.scale_outputs:
-                v = v.astype('float32')
+                v = v.astype("float32")
                 v /= scale_factor
 
             out[k] = v
 
         return out
 
     @out.setter
@@ -377,38 +396,38 @@
              - None is interpreted as a signal to clear the output dictionary.
         """
         if isinstance(result, list):
             # unpack futures list to dictionary first
             result = self.unpack_futures(result)
 
         if isinstance(result, dict):
-
             # iterate through dict where sites are keys and values are
             # corresponding results
             for site_gid, site_output in result.items():
-
                 # check that the sites are stored sequentially then add to
                 # the finished site list
                 if self._finished_sites:
                     if int(site_gid) < np.max(self._finished_sites):
-                        raise Exception('Site results are non sequential!')
+                        raise Exception("Site results are non sequential!")
 
                 # unpack site output object
                 self.unpack_output(site_gid, site_output)
 
                 # add site gid to the finished list after outputs are unpacked
                 self._finished_sites.append(site_gid)
 
         elif isinstance(result, type(None)):
             self._out.clear()
             self._finished_sites.clear()
         else:
-            raise TypeError('Did not recognize the type of output. '
-                            'Tried to set output type "{}", but requires '
-                            'list, dict or None.'.format(type(result)))
+            raise TypeError(
+                "Did not recognize the type of output. "
+                'Tried to set output type "{}", but requires '
+                "list, dict or None.".format(type(result))
+            )
 
     @staticmethod
     def _output_request_type_check(req):
         """Output request type check and ensure list for manipulation.
 
         Parameters
         ----------
@@ -424,16 +443,18 @@
         if isinstance(req, list):
             output_request = req
         elif isinstance(req, tuple):
             output_request = list(req)
         elif isinstance(req, str):
             output_request = [req]
         else:
-            raise TypeError('Output request must be str, list, or tuple but '
-                            'received: {}'.format(type(req)))
+            raise TypeError(
+                "Output request must be str, list, or tuple but "
+                "received: {}".format(type(req))
+            )
 
         return output_request
 
     @staticmethod
     def handle_leap_ti(ti, drop_leap=False):
         """Handle a time index for a leap year by dropping a day.
 
@@ -448,33 +469,42 @@
         Returns
         -------
         ti : pandas.DatetimeIndex
             Time-series datetime index with length a multiple of 365.
         """
 
         # Drop leap day or last day
-        leap_day = ((ti.month == 2) & (ti.day == 29))
+        leap_day = (ti.month == 2) & (ti.day == 29)
         leap_year = ti.year % 4 == 0
         last_day = ((ti.month == 12) & (ti.day == 31)) * leap_year
         if drop_leap:
             # Preference is to drop leap day if exists
             ti = ti.drop(ti[leap_day])
         elif any(leap_day):
             # Leap day exists but preference is to drop last day of year
             ti = ti.drop(ti[last_day])
 
         if len(ti) % 365 != 0:
-            raise ValueError('Bad time index with length not a multiple of '
-                             '365: {}'.format(ti))
+            raise ValueError(
+                "Bad time index with length not a multiple of "
+                "365: {}".format(ti)
+            )
 
         return ti
 
     @staticmethod
-    def _pp_to_pc(points, points_range, sam_configs, tech,
-                  sites_per_worker=None, res_file=None, curtailment=None):
+    def _pp_to_pc(
+        points,
+        points_range,
+        sam_configs,
+        tech,
+        sites_per_worker=None,
+        res_file=None,
+        curtailment=None,
+    ):
         """
         Create ProjectControl from ProjectPoints
 
         Parameters
         ----------
         points : int | slice | list | str | pandas.DataFrame
                  | reV.config.project_points.PointsControl
@@ -515,33 +545,50 @@
         -------
         pc : reV.config.project_points.PointsControl
             PointsControl object instance.
         """
         if hasattr(points, "df"):
             points = points.df
 
-        pp = ProjectPoints(points, sam_configs, tech=tech, res_file=res_file,
-                           curtailment=curtailment)
+        pp = ProjectPoints(
+            points,
+            sam_configs,
+            tech=tech,
+            res_file=res_file,
+            curtailment=curtailment,
+        )
 
         #  make Points Control instance
         if points_range is not None:
             # PointsControl is for just a subset of the project points...
             # this is the case if generation is being initialized on one
             # of many HPC nodes in a large project
-            pc = PointsControl.split(points_range[0], points_range[1], pp,
-                                     sites_per_split=sites_per_worker)
+            pc = PointsControl.split(
+                points_range[0],
+                points_range[1],
+                pp,
+                sites_per_split=sites_per_worker,
+            )
         else:
             # PointsControl is for all of the project points
             pc = PointsControl(pp, sites_per_split=sites_per_worker)
 
         return pc
 
     @classmethod
-    def get_pc(cls, points, points_range, sam_configs, tech,
-               sites_per_worker=None, res_file=None, curtailment=None):
+    def get_pc(
+        cls,
+        points,
+        points_range,
+        sam_configs,
+        tech,
+        sites_per_worker=None,
+        res_file=None,
+        curtailment=None,
+    ):
         """Get a PointsControl instance.
 
         Parameters
         ----------
         points : int | slice | list | str | pandas.DataFrame | PointsControl
             Single site integer,
             or slice or list specifying project points,
@@ -581,34 +628,46 @@
         Returns
         -------
         pc : reV.config.project_points.PointsControl
             PointsControl object instance.
         """
 
         if tech not in cls.OPTIONS and tech.lower() != ModuleName.ECON:
-            msg = ('Did not recognize reV-SAM technology string "{}". '
-                   'Technology string options are: {}'
-                   .format(tech, list(cls.OPTIONS.keys())))
+            msg = (
+                'Did not recognize reV-SAM technology string "{}". '
+                "Technology string options are: {}".format(
+                    tech, list(cls.OPTIONS.keys())
+                )
+            )
             logger.error(msg)
             raise KeyError(msg)
 
         if sites_per_worker is None:
             # get the optimal sites per split based on res file chunk size
             sites_per_worker = cls.get_sites_per_worker(res_file)
 
-        logger.debug('Sites per worker being set to {} for '
-                     'PointsControl.'.format(sites_per_worker))
+        logger.debug(
+            "Sites per worker being set to {} for " "PointsControl.".format(
+                sites_per_worker
+            )
+        )
 
         if isinstance(points, PointsControl):
             # received a pre-intialized instance of pointscontrol
             pc = points
         else:
-            pc = cls._pp_to_pc(points, points_range, sam_configs, tech,
-                               sites_per_worker=sites_per_worker,
-                               res_file=res_file, curtailment=curtailment)
+            pc = cls._pp_to_pc(
+                points,
+                points_range,
+                sam_configs,
+                tech,
+                sites_per_worker=sites_per_worker,
+                res_file=res_file,
+                curtailment=curtailment,
+            )
 
         return pc
 
     @staticmethod
     def get_sites_per_worker(res_file, default=100):
         """Get the nominal sites per worker (x-chunk size) for a given file.
 
@@ -633,39 +692,45 @@
             chunk size for windspeed and dni datasets for the WTK and NSRDB
             data, respectively.
         """
         if not res_file or not os.path.isfile(res_file):
             return default
 
         with Resource(res_file) as res:
-            if 'wtk' in res_file.lower():
+            if "wtk" in res_file.lower():
                 for dset in res.datasets:
-                    if 'speed' in dset:
+                    if "speed" in dset:
                         # take nominal WTK chunks from windspeed
                         _, _, chunks = res.get_dset_properties(dset)
                         break
-            elif 'nsrdb' in res_file.lower():
+            elif "nsrdb" in res_file.lower():
                 # take nominal NSRDB chunks from dni
-                _, _, chunks = res.get_dset_properties('dni')
+                _, _, chunks = res.get_dset_properties("dni")
             else:
-                warn('Could not infer dataset chunk size as the resource type '
-                     'could not be determined from the filename: {}'
-                     .format(res_file))
+                warn(
+                    "Could not infer dataset chunk size as the resource type "
+                    "could not be determined from the filename: {}".format(
+                        res_file
+                    )
+                )
                 chunks = None
 
         if chunks is None:
             # if chunks not set, go to default
             sites_per_worker = default
-            logger.debug('Sites per worker being set to {} (default) based on '
-                         'no set chunk size in {}.'
-                         .format(sites_per_worker, res_file))
+            logger.debug(
+                "Sites per worker being set to {} (default) based on "
+                "no set chunk size in {}.".format(sites_per_worker, res_file)
+            )
         else:
             sites_per_worker = chunks[1]
-            logger.debug('Sites per worker being set to {} based on chunk '
-                         'size of {}.'.format(sites_per_worker, res_file))
+            logger.debug(
+                "Sites per worker being set to {} based on chunk "
+                "size of {}.".format(sites_per_worker, res_file)
+            )
 
         return sites_per_worker
 
     @staticmethod
     def unpack_futures(futures):
         """Combine list of futures results into their native dict format/type.
 
@@ -684,16 +749,21 @@
         for x in futures:
             out.update(x)
 
         return out
 
     @staticmethod
     @abstractmethod
-    def _run_single_worker(points_control, tech=None, res_file=None,
-                           output_request=None, scale_outputs=True):
+    def _run_single_worker(
+        points_control,
+        tech=None,
+        res_file=None,
+        output_request=None,
+        scale_outputs=True,
+    ):
         """Run a reV-SAM analysis based on the points_control iterator.
 
         Parameters
         ----------
         points_control : reV.config.PointsControl
             A PointsControl instance dictating what sites and configs are run.
         tech : str
@@ -731,39 +801,45 @@
             Site-specific data for econ calculation. Rows correspond to sites,
             columns are variables.
         """
 
         if inp is None or inp is False:
             # no input, just initialize dataframe with site gids as index
             site_data = pd.DataFrame(index=self.project_points.sites)
-            site_data.index.name = 'gid'
+            site_data.index.name = ResourceMetaField.GID
         else:
             # explicit input, initialize df
             if isinstance(inp, str):
-                if inp.endswith('.csv'):
+                if inp.endswith(".csv"):
                     site_data = pd.read_csv(inp)
             elif isinstance(inp, pd.DataFrame):
                 site_data = inp
             else:
                 # site data was not able to be set. Raise error.
-                raise Exception('Site data input must be .csv or '
-                                'dataframe, but received: {}'.format(inp))
-
-            if 'gid' not in site_data and site_data.index.name != 'gid':
+                raise Exception(
+                    "Site data input must be .csv or "
+                    "dataframe, but received: {}".format(inp)
+                )
+
+            gid_not_in_site_data = ResourceMetaField.GID not in site_data
+            index_name_not_gid = site_data.index.name != ResourceMetaField.GID
+            if gid_not_in_site_data and index_name_not_gid:
                 # require gid as column label or index
-                raise KeyError('Site data input must have "gid" column '
-                               'to match reV site gid.')
+                raise KeyError('Site data input must have '
+                               f'{ResourceMetaField.GID} column to match '
+                               'reV site gid.')
 
             # pylint: disable=no-member
-            if site_data.index.name != 'gid':
+            if site_data.index.name != ResourceMetaField.GID:
                 # make gid the dataframe index if not already
-                site_data = site_data.set_index('gid', drop=True)
+                site_data = site_data.set_index(ResourceMetaField.GID,
+                                                drop=True)
 
-        if 'offshore' in site_data:
-            if site_data['offshore'].sum() > 1:
+        if "offshore" in site_data:
+            if site_data["offshore"].sum() > 1:
                 w = ('Found offshore sites in econ site data input. '
                      'This functionality has been deprecated. '
                      'Please run the reV offshore module to '
                      'calculate offshore wind lcoe.')
                 warn(w, OffshoreWindInputWarning)
                 logger.warning(w)
 
@@ -820,44 +896,49 @@
         if dset in self.project_points.all_sam_input_keys:
             return self._get_data_shape_from_sam_config(dset, n_sites)
 
         return self._get_data_shape_from_pysam(dset, n_sites)
 
     def _get_data_shape_from_out_attrs(self, dset, n_sites):
         """Get data shape from ``OUT_ATTRS`` variable"""
-        if self.OUT_ATTRS[dset]['type'] == 'array':
+        if self.OUT_ATTRS[dset]["type"] == "array":
             return (len(self.time_index), n_sites)
         return (n_sites,)
 
     def _get_data_shape_from_sam_config(self, dset, n_sites):
-        """Get data shape from SAM input config """
+        """Get data shape from SAM input config"""
         data = list(self.project_points.sam_inputs.values())[0][dset]
         if isinstance(data, (list, tuple, np.ndarray)):
             return (*np.array(data).shape, n_sites)
 
         if isinstance(data, str):
-            msg = ('Cannot pass through non-scalar SAM input key "{}" '
-                   'as an output_request!'.format(dset))
+            msg = (
+                'Cannot pass through non-scalar SAM input key "{}" '
+                "as an output_request!".format(dset)
+            )
             logger.error(msg)
             raise ExecutionError(msg)
 
-        return (n_sites, )
+        return (n_sites,)
 
     def _get_data_shape_from_pysam(self, dset, n_sites):
         """Get data shape from PySAM output object"""
         if self._sam_obj_default is None:
             self._sam_obj_default = self.sam_module.default()
 
         try:
             out_data = getattr(self._sam_obj_default.Outputs, dset)
         except AttributeError as e:
-            msg = ('Could not get data shape for dset "{}" '
-                   'from object "{}". '
-                   'Received the following error: "{}"'
-                   .format(dset, self._sam_obj_default, e))
+            msg = (
+                'Could not get data shape for dset "{}" '
+                'from object "{}". '
+                'Received the following error: "{}"'.format(
+                    dset, self._sam_obj_default, e
+                )
+            )
             logger.error(msg)
             raise ExecutionError(msg) from e
 
         if isinstance(out_data, (int, float, str)):
             return (n_sites,)
 
         if len(out_data) % len(self.time_index) == 0:
@@ -869,86 +950,101 @@
         """Combine directory and filename, ensure .h5 ext., make out dirs."""
         if out_fpath is None:
             return
 
         project_dir, out_fn = os.path.split(out_fpath)
 
         # ensure output file is an h5
-        if not out_fn.endswith('.h5'):
-            out_fn += '.h5'
+        if not out_fn.endswith(".h5"):
+            out_fn += ".h5"
 
         if module not in out_fn:
             extension_with_module = "_{}.h5".format(module)
             out_fn = out_fn.replace(".h5", extension_with_module)
 
         # ensure year is in out_fpath
-        if self.year is not None and str(self.year) not in out_fn:
+        if self.year is not None:
             extension_with_year = "_{}.h5".format(self.year)
-            out_fn = out_fn.replace(".h5", extension_with_year)
+            if extension_with_year not in out_fn:
+                out_fn = out_fn.replace(".h5", extension_with_year)
 
         # create and use optional output dir
         if project_dir and not os.path.exists(project_dir):
             os.makedirs(project_dir, exist_ok=True)
 
         self._out_fpath = os.path.join(project_dir, out_fn)
-        self._run_attrs['out_fpath'] = out_fpath
+        self._run_attrs["out_fpath"] = out_fpath
 
-    def _init_h5(self, mode='w'):
+    def _init_h5(self, mode="w"):
         """Initialize the single h5 output file with all output requests.
 
         Parameters
         ----------
         mode : str
             Mode to instantiate h5py.File instance
         """
 
         if self._out_fpath is None:
             return
 
-        if 'w' in mode:
-            logger.info('Initializing full output file: "{}" with mode: {}'
-                        .format(self._out_fpath, mode))
-        elif 'a' in mode:
-            logger.info('Appending data to output file: "{}" with mode: {}'
-                        .format(self._out_fpath, mode))
+        if "w" in mode:
+            logger.info(
+                'Initializing full output file: "{}" with mode: {}'.format(
+                    self._out_fpath, mode
+                )
+            )
+        elif "a" in mode:
+            logger.info(
+                'Appending data to output file: "{}" with mode: {}'.format(
+                    self._out_fpath, mode
+                )
+            )
 
         attrs = {d: {} for d in self.output_request}
         chunks = {}
         dtypes = {}
         shapes = {}
 
         # flag to write time index if profiles are being output
         write_ti = False
 
         for dset in self.output_request:
-
-            tmp = 'other'
+            tmp = "other"
             if dset in self.OUT_ATTRS:
                 tmp = dset
 
-            attrs[dset]['units'] = self.OUT_ATTRS[tmp].get('units',
-                                                           'unknown')
-            attrs[dset]['scale_factor'] = \
-                self.OUT_ATTRS[tmp].get('scale_factor', 1)
-            chunks[dset] = self.OUT_ATTRS[tmp].get('chunks', None)
-            dtypes[dset] = self.OUT_ATTRS[tmp].get('dtype', 'float32')
+            attrs[dset]["units"] = self.OUT_ATTRS[tmp].get("units", "unknown")
+            attrs[dset]["scale_factor"] = self.OUT_ATTRS[tmp].get(
+                "scale_factor", 1
+            )
+            chunks[dset] = self.OUT_ATTRS[tmp].get("chunks", None)
+            dtypes[dset] = self.OUT_ATTRS[tmp].get("dtype", "float32")
             shapes[dset] = self._get_data_shape(dset, len(self.meta))
             if len(shapes[dset]) > 1:
                 write_ti = True
 
         # only write time index if profiles were found in output request
         if write_ti:
             ti = self.time_index
         else:
             ti = None
 
-        Outputs.init_h5(self._out_fpath, self.output_request, shapes,
-                        attrs, chunks, dtypes, self.meta, time_index=ti,
-                        configs=self.sam_metas, run_attrs=self.run_attrs,
-                        mode=mode)
+        Outputs.init_h5(
+            self._out_fpath,
+            self.output_request,
+            shapes,
+            attrs,
+            chunks,
+            dtypes,
+            self.meta,
+            time_index=ti,
+            configs=self.sam_metas,
+            run_attrs=self.run_attrs,
+            mode=mode,
+        )
 
     def _init_out_arrays(self, index_0=0):
         """Initialize output arrays based on the number of sites that can be
         stored in memory safely.
 
         Parameters
         ----------
@@ -958,29 +1054,35 @@
             this is used to segment the sites in the current output chunk.
         """
 
         self._out = {}
         self._finished_sites = []
 
         # Output chunk is the index range (inclusive) of this set of site outs
-        self._out_chunk = (index_0, np.min((index_0 + self.site_limit,
-                                            len(self.project_points) - 1)))
+        self._out_chunk = (
+            index_0,
+            np.min((index_0 + self.site_limit, len(self.project_points) - 1)),
+        )
         self._out_n_sites = int(self.out_chunk[1] - self.out_chunk[0]) + 1
 
-        logger.info('Initializing in-memory outputs for {} sites with gids '
-                    '{} through {} inclusive (site list index {} through {})'
-                    .format(self._out_n_sites,
-                            self.project_points.sites[self.out_chunk[0]],
-                            self.project_points.sites[self.out_chunk[1]],
-                            self.out_chunk[0], self.out_chunk[1]))
+        logger.info(
+            "Initializing in-memory outputs for {} sites with gids "
+            "{} through {} inclusive (site list index {} through {})".format(
+                self._out_n_sites,
+                self.project_points.sites[self.out_chunk[0]],
+                self.project_points.sites[self.out_chunk[1]],
+                self.out_chunk[0],
+                self.out_chunk[1],
+            )
+        )
 
         for request in self.output_request:
-            dtype = 'float32'
+            dtype = "float32"
             if request in self.OUT_ATTRS and self.scale_outputs:
-                dtype = self.OUT_ATTRS[request].get('dtype', 'float32')
+                dtype = self.OUT_ATTRS[request].get("dtype", "float32")
 
             shape = self._get_data_shape(request, self._out_n_sites)
 
             # initialize the output request as an array of zeros
             self._out[request] = np.zeros(shape, dtype=dtype)
 
     def _check_sam_version_inputs(self):
@@ -1000,17 +1102,19 @@
         site_output : dict
             SAM site output object.
         """
 
         # iterate through the site results
         for var, value in site_output.items():
             if var not in self._out:
-                raise KeyError('Tried to collect output variable "{}", but it '
-                               'was not yet initialized in the output '
-                               'dictionary.')
+                raise KeyError(
+                    'Tried to collect output variable "{}", but it '
+                    "was not yet initialized in the output "
+                    "dictionary."
+                )
 
             # get the index in the output array for the current site
             i = self.site_index(site_gid, out_index=True)
 
             # check to see if we have exceeded the current output chunk.
             # If so, flush data to disk and reset the output initialization
             if i + 1 > self._out_n_sites:
@@ -1051,53 +1155,57 @@
         global_site_index = self.project_points.sites.index(site_gid)
 
         if not out_index:
             output_index = global_site_index
         else:
             output_index = global_site_index - self.out_chunk[0]
             if output_index < 0:
-                raise ValueError('Attempting to set output data for site with '
-                                 'gid {} to global site index {}, which was '
-                                 'already set based on the current output '
-                                 'index chunk of {}'
-                                 .format(site_gid, global_site_index,
-                                         self.out_chunk))
+                raise ValueError(
+                    "Attempting to set output data for site with "
+                    "gid {} to global site index {}, which was "
+                    "already set based on the current output "
+                    "index chunk of {}".format(
+                        site_gid, global_site_index, self.out_chunk
+                    )
+                )
 
         return output_index
 
     def flush(self):
         """Flush the output data in self.out attribute to disk in .h5 format.
 
         The data to be flushed is accessed from the instance attribute
         "self.out". The disk target is based on the instance attributes
         "self._out_fpath". Data is not flushed if _fpath is None or if .out is
         empty.
         """
 
         # handle output file request if file is specified and .out is not empty
         if isinstance(self._out_fpath, str) and self._out:
-            logger.info('Flushing outputs to disk, target file: "{}"'
-                        .format(self._out_fpath))
+            logger.info(
+                'Flushing outputs to disk, target file: "{}"'.format(
+                    self._out_fpath
+                )
+            )
 
             # get the slice of indices to write outputs to
             islice = slice(self.out_chunk[0], self.out_chunk[1] + 1)
 
             # open output file in append mode to add output results to
-            with Outputs(self._out_fpath, mode='a') as f:
-
+            with Outputs(self._out_fpath, mode="a") as f:
                 # iterate through all output requests writing each as a dataset
                 for dset, arr in self._out.items():
                     if len(arr.shape) == 1:
                         # write array of scalars
                         f[dset, islice] = arr
                     else:
                         # write 2D array of profiles
                         f[dset, :, islice] = arr
 
-            logger.debug('Flushed output successfully to disk.')
+            logger.debug("Flushed output successfully to disk.")
 
     def _pre_split_pc(self, pool_size=None):
         """Pre-split project control iterator into sub chunks to further
         split the parallelization.
 
         Parameters
         ----------
@@ -1125,19 +1233,23 @@
             if (i + 1) % pool_size == 0:
                 pc_chunks.append(i_chunk)
                 i_chunk = []
 
         if i_chunk:
             pc_chunks.append(i_chunk)
 
-        logger.debug('Pre-splitting points control into {} chunks with the '
-                     'following chunk sizes: {}'
-                     .format(len(pc_chunks), [len(x) for x in pc_chunks]))
+        logger.debug(
+            "Pre-splitting points control into {} chunks with the "
+            "following chunk sizes: {}".format(
+                len(pc_chunks), [len(x) for x in pc_chunks]
+            )
+        )
         return N, pc_chunks
 
+    # pylint: disable=unused-argument
     def _reduce_kwargs(self, pc, **kwargs):
         """Placeholder for functions that need to reduce the global kwargs that
         they send to workers to reduce memory footprint
 
         Parameters
         ----------
         pc : PointsControl
@@ -1149,16 +1261,17 @@
         Returns
         -------
         kwargs : dict
             Same as input but reduced just for the gids in pc
         """
         return kwargs
 
-    def _parallel_run(self, max_workers=None, pool_size=None, timeout=1800,
-                      **kwargs):
+    def _parallel_run(
+        self, max_workers=None, pool_size=None, timeout=1800, **kwargs
+    ):
         """Execute parallel compute.
 
         Parameters
         ----------
         max_workers : None | int
             Number of workers. None will default to cpu count.
         pool_size : int
@@ -1172,61 +1285,75 @@
             Keyword arguments to self._run_single_worker().
         """
 
         if pool_size is None:
             pool_size = os.cpu_count() * 2
         if max_workers is None:
             max_workers = os.cpu_count()
-        logger.info('Running parallel execution with max_workers={}'
-                    .format(max_workers))
+        logger.info(
+            "Running parallel execution with max_workers={}".format(
+                max_workers
+            )
+        )
         i = 0
         N, pc_chunks = self._pre_split_pc(pool_size=pool_size)
         for j, pc_chunk in enumerate(pc_chunks):
-            logger.debug('Starting process pool for points control '
-                         'iteration {} out of {}'
-                         .format(j + 1, len(pc_chunks)))
+            logger.debug(
+                "Starting process pool for points control "
+                "iteration {} out of {}".format(j + 1, len(pc_chunks))
+            )
 
             failed_futures = False
             chunks = {}
             futures = []
-            loggers = [__name__, 'reV.gen', 'reV.econ', 'reV']
-            with SpawnProcessPool(max_workers=max_workers,
-                                  loggers=loggers) as exe:
+            loggers = [__name__, "reV.gen", "reV.econ", "reV"]
+            with SpawnProcessPool(
+                max_workers=max_workers, loggers=loggers
+            ) as exe:
                 for pc in pc_chunk:
                     pc_kwargs = self._reduce_kwargs(pc, **kwargs)
-                    future = exe.submit(self._run_single_worker, pc,
-                                        **pc_kwargs)
+                    future = exe.submit(
+                        self._run_single_worker, pc, **pc_kwargs
+                    )
                     futures.append(future)
                     chunks[future] = pc
 
                 for future in futures:
                     i += 1
                     try:
                         result = future.result(timeout=timeout)
                     except TimeoutError:
                         failed_futures = True
                         sites = chunks[future].project_points.sites
-                        result = self._handle_failed_future(future, i, sites,
-                                                            timeout)
+                        result = self._handle_failed_future(
+                            future, i, sites, timeout
+                        )
 
                     self.out = result
 
                     mem = psutil.virtual_memory()
-                    m = ('Parallel run at iteration {0} out of {1}. '
-                         'Memory utilization is {2:.3f} GB out of {3:.3f} GB '
-                         'total ({4:.1f}% used, intended limit of {5:.1f}%)'
-                         .format(i, N, mem.used / 1e9, mem.total / 1e9,
-                                 100 * mem.used / mem.total,
-                                 100 * self.mem_util_lim))
+                    m = (
+                        "Parallel run at iteration {0} out of {1}. "
+                        "Memory utilization is {2:.3f} GB out of {3:.3f} GB "
+                        "total ({4:.1f}% used, intended limit of {5:.1f}%)"
+                        .format(
+                            i,
+                            N,
+                            mem.used / 1e9,
+                            mem.total / 1e9,
+                            100 * mem.used / mem.total,
+                            100 * self.mem_util_lim,
+                        )
+                    )
                     logger.info(m)
 
                 if failed_futures:
-                    logger.info('Forcing pool shutdown after failed futures.')
+                    logger.info("Forcing pool shutdown after failed futures.")
                     exe.shutdown(wait=False)
-                    logger.info('Forced pool shutdown complete.')
+                    logger.info("Forced pool shutdown complete.")
 
         self.flush()
 
     def _handle_failed_future(self, future, i, sites, timeout):
         """Handle a failed future and return zeros.
 
         Parameters
@@ -1238,28 +1365,28 @@
         sites : list
             List of site gids belonging to this failed future.
         timeout : int
             Number of seconds to wait for parallel run iteration to complete
             before returning zeros.
         """
 
-        w = ('Iteration {} hit the timeout limit of {} seconds! Passing zeros.'
-             .format(i, timeout))
+        w = ("Iteration {} hit the timeout limit of {} seconds! "
+             "Passing zeros.".format(i, timeout))
         logger.warning(w)
         warn(w, OutputWarning)
 
-        site_out = {k: 0 for k in self.output_request}
-        result = {site: site_out for site in sites}
+        site_out = dict.fromkeys(self.output_request, 0)
+        result = dict.fromkeys(sites, site_out)
 
         try:
             cancelled = future.cancel()
         except Exception as e:
-            w = 'Could not cancel future! Received exception: {}'.format(e)
+            w = "Could not cancel future! Received exception: {}".format(e)
             logger.warning(w)
             warn(w, ParallelExecutionWarning)
 
         if not cancelled:
-            w = 'Could not cancel future!'
+            w = "Could not cancel future!"
             logger.warning(w)
             warn(w, ParallelExecutionWarning)
 
         return result
```

### Comparing `NREL-reV-0.8.7/reV/generation/cli_gen.py` & `NREL-reV-0.8.9/reV/generation/cli_gen.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/generation/generation.py` & `NREL-reV-0.8.9/reV/generation/generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,111 @@
 # -*- coding: utf-8 -*-
 """
 reV generation module.
 """
+
 import copy
 import json
 import logging
 import os
 import pprint
 
 import numpy as np
 import pandas as pd
-
-from reV.generation.base import BaseGen
-from reV.SAM.generation import (Geothermal,
-                                MhkWave,
-                                LinearDirectSteam,
-                                PvSamv1,
-                                PvWattsv5,
-                                PvWattsv7,
-                                PvWattsv8,
-                                SolarWaterHeat,
-                                TcsMoltenSalt,
-                                TroughPhysicalHeat,
-                                WindPower)
-from reV.utilities import ModuleName
-from reV.utilities.exceptions import (ConfigError,
-                                      InputError,
-                                      ProjectPointsValueError)
 from rex.multi_file_resource import MultiFileResource
 from rex.multi_res_resource import MultiResolutionResource
 from rex.resource import Resource
 from rex.utilities.utilities import check_res_file
 
+from reV.generation.base import BaseGen
+from reV.SAM.generation import (
+    Geothermal,
+    LinearDirectSteam,
+    MhkWave,
+    PvSamv1,
+    PvWattsv5,
+    PvWattsv7,
+    PvWattsv8,
+    SolarWaterHeat,
+    TcsMoltenSalt,
+    TroughPhysicalHeat,
+    WindPower,
+)
+from reV.utilities import ModuleName, ResourceMetaField, SupplyCurveField
+from reV.utilities.exceptions import (
+    ConfigError,
+    InputError,
+    ProjectPointsValueError,
+)
+
 logger = logging.getLogger(__name__)
 
 
 ATTR_DIR = os.path.dirname(os.path.realpath(__file__))
-ATTR_DIR = os.path.join(ATTR_DIR, 'output_attributes')
-with open(os.path.join(ATTR_DIR, 'other.json'), 'r') as f:
+ATTR_DIR = os.path.join(ATTR_DIR, "output_attributes")
+with open(os.path.join(ATTR_DIR, "other.json")) as f:
     OTHER_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'generation.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, "generation.json")) as f:
     GEN_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'linear_fresnel.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, "linear_fresnel.json")) as f:
     LIN_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'solar_water_heat.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, "solar_water_heat.json")) as f:
     SWH_ATTRS = json.load(f)
-with open(os.path.join(ATTR_DIR, 'trough_heat.json'), 'r') as f:
+with open(os.path.join(ATTR_DIR, "trough_heat.json")) as f:
     TPPH_ATTRS = json.load(f)
 
 
 class Gen(BaseGen):
     """Gen"""
 
     # Mapping of reV technology strings to SAM generation objects
-    OPTIONS = {'geothermal': Geothermal,
-               'lineardirectsteam': LinearDirectSteam,
-               'mhkwave': MhkWave,
-               'pvsamv1': PvSamv1,
-               'pvwattsv5': PvWattsv5,
-               'pvwattsv7': PvWattsv7,
-               'pvwattsv8': PvWattsv8,
-               'solarwaterheat': SolarWaterHeat,
-               'tcsmoltensalt': TcsMoltenSalt,
-               'troughphysicalheat': TroughPhysicalHeat,
-               'windpower': WindPower}
+    OPTIONS = {
+        "geothermal": Geothermal,
+        "lineardirectsteam": LinearDirectSteam,
+        "mhkwave": MhkWave,
+        "pvsamv1": PvSamv1,
+        "pvwattsv5": PvWattsv5,
+        "pvwattsv7": PvWattsv7,
+        "pvwattsv8": PvWattsv8,
+        "solarwaterheat": SolarWaterHeat,
+        "tcsmoltensalt": TcsMoltenSalt,
+        "troughphysicalheat": TroughPhysicalHeat,
+        "windpower": WindPower,
+    }
 
     """reV technology options."""
 
     # Mapping of reV generation outputs to scale factors and units.
     # Type is scalar or array and corresponds to the SAM single-site output
     OUT_ATTRS = copy.deepcopy(OTHER_ATTRS)
     OUT_ATTRS.update(GEN_ATTRS)
     OUT_ATTRS.update(LIN_ATTRS)
     OUT_ATTRS.update(SWH_ATTRS)
     OUT_ATTRS.update(TPPH_ATTRS)
     OUT_ATTRS.update(BaseGen.ECON_ATTRS)
 
-    def __init__(self, technology, project_points, sam_files, resource_file,
-                 low_res_resource_file=None, output_request=('cf_mean',),
-                 site_data=None, curtailment=None, gid_map=None,
-                 drop_leap=False, sites_per_worker=None,
-                 memory_utilization_limit=0.4, scale_outputs=True,
-                 write_mapped_gids=False, bias_correct=None):
-        """reV generation analysis class.
+    def __init__(
+        self,
+        technology,
+        project_points,
+        sam_files,
+        resource_file,
+        low_res_resource_file=None,
+        output_request=("cf_mean",),
+        site_data=None,
+        curtailment=None,
+        gid_map=None,
+        drop_leap=False,
+        sites_per_worker=None,
+        memory_utilization_limit=0.4,
+        scale_outputs=True,
+        write_mapped_gids=False,
+        bias_correct=None,
+    ):
+        """ReV generation analysis class.
 
         ``reV`` generation analysis runs SAM simulations by piping in
         renewable energy resource data (usually from the NSRDB or WTK),
         loading the SAM config, and then executing the PySAM compute
         module for a given technology. See the documentation for the
         ``reV`` SAM class (e.g. :class:`reV.SAM.generation.WindPower`,
         :class:`reV.SAM.generation.PvWattsv8`,
@@ -117,22 +136,22 @@
         >>> gen = Gen(sam_tech, sites, fp_sam, fp_res)
         >>> gen.run()
         >>>
         >>> gen.out
         {'cf_mean': array([0.16966143], dtype=float32)}
         >>>
         >>> sites = [3, 4, 7, 9]
-        >>> req = ('cf_mean', 'cf_profile', 'lcoe_fcr')
+        >>> req = ('cf_mean', 'lcoe_fcr')
         >>> gen = Gen(sam_tech, sites, fp_sam, fp_res, output_request=req)
         >>> gen.run()
         >>>
         >>> gen.out
         {'lcoe_fcr': array([131.39166, 131.31221, 127.54539, 125.49656]),
-        'cf_mean': array([0.17713654, 0.17724372, 0.1824783 , 0.1854574 ]),
-        'cf_profile': array([[0., 0., 0., 0.],
+         'cf_mean': array([0.17713654, 0.17724372, 0.1824783 , 0.1854574 ]),
+        : array([[0., 0., 0., 0.],
                 [0., 0., 0., 0.],
                 [0., 0., 0., 0.],
                 ...,
                 [0., 0., 0., 0.],
                 [0., 0., 0., 0.],
                 [0., 0., 0., 0.]])}
 
@@ -357,39 +376,50 @@
             inputs for ``method``. Any additional kwargs required for the
             requested ``method`` can be input as additional columns in the
             ``bias_correct`` table e.g., for linear bias correction functions
             you can include ``scalar`` and ``adder`` inputs as columns in the
             ``bias_correct`` table on a site-by-site basis. If ``None``, no
             corrections are applied. By default, ``None``.
         """
-        pc = self.get_pc(points=project_points, points_range=None,
-                         sam_configs=sam_files, tech=technology,
-                         sites_per_worker=sites_per_worker,
-                         res_file=resource_file,
-                         curtailment=curtailment)
-
-        super().__init__(pc, output_request, site_data=site_data,
-                         drop_leap=drop_leap,
-                         memory_utilization_limit=memory_utilization_limit,
-                         scale_outputs=scale_outputs)
+        pc = self.get_pc(
+            points=project_points,
+            points_range=None,
+            sam_configs=sam_files,
+            tech=technology,
+            sites_per_worker=sites_per_worker,
+            res_file=resource_file,
+            curtailment=curtailment,
+        )
+
+        super().__init__(
+            pc,
+            output_request,
+            site_data=site_data,
+            drop_leap=drop_leap,
+            memory_utilization_limit=memory_utilization_limit,
+            scale_outputs=scale_outputs,
+        )
 
         if self.tech not in self.OPTIONS:
-            msg = ('Requested technology "{}" is not available. '
-                   'reV generation can analyze the following '
-                   'SAM technologies: {}'
-                   .format(self.tech, list(self.OPTIONS.keys())))
+            msg = (
+                'Requested technology "{}" is not available. '
+                "reV generation can analyze the following "
+                "SAM technologies: {}".format(
+                    self.tech, list(self.OPTIONS.keys())
+                )
+            )
             logger.error(msg)
             raise KeyError(msg)
 
         self.write_mapped_gids = write_mapped_gids
         self._res_file = resource_file
         self._lr_res_file = low_res_resource_file
         self._sam_module = self.OPTIONS[self.tech]
-        self._run_attrs['sam_module'] = self._sam_module.MODULE
-        self._run_attrs['res_file'] = resource_file
+        self._run_attrs["sam_module"] = self._sam_module.MODULE
+        self._run_attrs["res_file"] = resource_file
 
         self._multi_h5_res, self._hsds = check_res_file(resource_file)
         self._gid_map = self._parse_gid_map(gid_map)
         self._nn_map = self._parse_nn_map()
         self._bc = self._parse_bc(bias_correct)
 
     @property
@@ -420,47 +450,51 @@
 
         Returns
         -------
         meta : pd.DataFrame
             Meta data df for sites in project points. Column names are meta
             data variables, rows are different sites. The row index
             does not indicate the site number if the project points are
-            non-sequential or do not start from 0, so a 'gid' column is added.
+            non-sequential or do not start from 0, so a `SupplyCurveField.GID`
+            column is added.
         """
         if self._meta is None:
             res_cls = Resource
-            kwargs = {'hsds': self._hsds}
+            kwargs = {"hsds": self._hsds}
             if self._multi_h5_res:
                 res_cls = MultiFileResource
                 kwargs = {}
 
             res_gids = self.project_points.sites
             if self._gid_map is not None:
                 res_gids = [self._gid_map[i] for i in res_gids]
 
             with res_cls(self.res_file, **kwargs) as res:
-                meta_len = res.shapes['meta'][0]
+                meta_len = res.shapes["meta"][0]
 
                 if np.max(res_gids) > meta_len:
-                    msg = ('ProjectPoints has a max site gid of {} which is '
-                           'out of bounds for the meta data of len {} from '
-                           'resource file: {}'
-                           .format(np.max(res_gids),
-                                   meta_len, self.res_file))
+                    msg = (
+                        "ProjectPoints has a max site gid of {} which is "
+                        "out of bounds for the meta data of len {} from "
+                        "resource file: {}".format(
+                            np.max(res_gids), meta_len, self.res_file
+                        )
+                    )
                     logger.error(msg)
                     raise ProjectPointsValueError(msg)
 
-                self._meta = res['meta', res_gids]
+                self._meta = res["meta", res_gids]
 
-            self._meta.loc[:, 'gid'] = res_gids
+            self._meta.loc[:, ResourceMetaField.GID] = res_gids
             if self.write_mapped_gids:
-                self._meta.loc[:, 'gid'] = self.project_points.sites
+                sites = self.project_points.sites
+                self._meta.loc[:, ResourceMetaField.GID] = sites
             self._meta.index = self.project_points.sites
-            self._meta.index.name = 'gid'
-            self._meta.loc[:, 'reV_tech'] = self.project_points.tech
+            self._meta.index.name = ResourceMetaField.GID
+            self._meta.loc[:, "reV_tech"] = self.project_points.tech
 
         return self._meta
 
     @property
     def time_index(self):
         """Get the generation resource time index data.
 
@@ -468,39 +502,42 @@
         -------
         _time_index : pandas.DatetimeIndex
             Time-series datetime index
         """
         if self._time_index is None:
             if not self._multi_h5_res:
                 res_cls = Resource
-                kwargs = {'hsds': self._hsds}
+                kwargs = {"hsds": self._hsds}
             else:
                 res_cls = MultiFileResource
                 kwargs = {}
 
             with res_cls(self.res_file, **kwargs) as res:
                 time_index = res.time_index
 
             downscale = self.project_points.sam_config_obj.downscale
             step = self.project_points.sam_config_obj.time_index_step
             if downscale is not None:
                 from rex.utilities.downscale import make_time_index
+
                 year = time_index.year[0]
-                ds_freq = downscale['frequency']
+                ds_freq = downscale["frequency"]
                 time_index = make_time_index(year, ds_freq)
-                logger.info('reV solar generation running with temporal '
-                            'downscaling frequency "{}" with final '
-                            'time_index length {}'
-                            .format(ds_freq, len(time_index)))
+                logger.info(
+                    "reV solar generation running with temporal "
+                    'downscaling frequency "{}" with final '
+                    "time_index length {}".format(ds_freq, len(time_index))
+                )
             elif step is not None:
                 time_index = time_index[::step]
 
             time_index = self.handle_lifetime_index(time_index)
-            time_index = self.handle_leap_ti(time_index,
-                                             drop_leap=self._drop_leap)
+            time_index = self.handle_leap_ti(
+                time_index, drop_leap=self._drop_leap
+            )
 
             self._time_index = time_index
 
         return self._time_index
 
     def handle_lifetime_index(self, ti):
         """Adjust the time index if modeling full system lifetime.
@@ -526,61 +563,73 @@
 
         if not any(ltp > 1 for ltp in lifetime_periods):
             return ti
 
         # Only one time index may be passed, check that lifetime periods match
         n_unique_periods = len(np.unique(lifetime_periods))
         if n_unique_periods != 1:
-            msg = ('reV cannot handle multiple analysis_periods when '
-                   'modeling with `system_use_lifetime_output` set '
-                   'to 1. Found {} different analysis_periods in the SAM '
-                   'configs'.format(n_unique_periods))
+            msg = (
+                "reV cannot handle multiple analysis_periods when "
+                "modeling with `system_use_lifetime_output` set "
+                "to 1. Found {} different analysis_periods in the SAM "
+                "configs".format(n_unique_periods)
+            )
             logger.error(msg)
             raise ConfigError(msg)
 
         # Collect requested variables to check for lifetime compatibility
         array_vars = [
-            var for var, attrs in GEN_ATTRS.items()
-            if attrs['type'] == 'array'
+            var for var, attrs in GEN_ATTRS.items() if attrs["type"] == "array"
         ]
-        valid_vars = ['gen_profile', 'cf_profile', 'cf_profile_ac']
+        valid_vars = ["gen_profile", "cf_profile", "cf_profile_ac"]
         invalid_vars = set(array_vars) - set(valid_vars)
-        invalid_requests = [var for var in self.output_request
-                            if var in invalid_vars]
+        invalid_requests = [
+            var for var in self.output_request if var in invalid_vars
+        ]
 
         if invalid_requests:
             # SAM does not output full lifetime for all array variables
             msg = (
-                'reV can only handle the following output arrays '
-                'when modeling with `system_use_lifetime_output` set '
-                'to 1: {}. Try running without {}.'.format(
-                    ', '.join(valid_vars), ', '.join(invalid_requests)
+                "reV can only handle the following output arrays "
+                "when modeling with `system_use_lifetime_output` set "
+                "to 1: {}. Try running without {}.".format(
+                    ", ".join(valid_vars), ", ".join(invalid_requests)
                 )
             )
             logger.error(msg)
             raise ConfigError(msg)
 
         sam_meta = self.sam_metas[next(iter(self.sam_metas))]
         analysis_period = sam_meta["analysis_period"]
-        logger.info('reV generation running with a full system '
-                    'life of {} years.'.format(analysis_period))
+        logger.info(
+            "reV generation running with a full system "
+            "life of {} years.".format(analysis_period)
+        )
 
         old_end = ti[-1]
         new_end = old_end + pd.DateOffset(years=analysis_period - 1)
         step = old_end - ti[-2]
         time_extension = pd.date_range(old_end, new_end, freq=step)
         ti = time_extension.union(ti)
 
         return ti
 
     @classmethod
-    def _run_single_worker(cls, points_control, tech=None, res_file=None,
-                           lr_res_file=None, output_request=None,
-                           scale_outputs=True, gid_map=None, nn_map=None,
-                           bias_correct=None):
+    def _run_single_worker(
+        cls,
+        points_control,
+        tech=None,
+        res_file=None,
+        lr_res_file=None,
+        output_request=None,
+        scale_outputs=True,
+        gid_map=None,
+        nn_map=None,
+        bias_correct=None,
+    ):
         """Run a SAM generation analysis based on the points_control iterator.
 
         Parameters
         ----------
         points_control : reV.config.PointsControl
             A PointsControl instance dictating what sites and configs are run.
         tech : str
@@ -633,55 +682,59 @@
         out : dict
             Output dictionary from the SAM reV_run function. Data is scaled
             within this function to the datatype specified in Gen.OUT_ATTRS.
         """
 
         # Extract the site df from the project points df.
         site_df = points_control.project_points.df
-        site_df = site_df.set_index('gid', drop=True)
+        site_df = site_df.set_index(ResourceMetaField.GID, drop=True)
 
         # run generation method for specified technology
         try:
             out = cls.OPTIONS[tech].reV_run(
-                points_control, res_file, site_df,
+                points_control,
+                res_file,
+                site_df,
                 lr_res_file=lr_res_file,
                 output_request=output_request,
-                gid_map=gid_map, nn_map=nn_map,
-                bias_correct=bias_correct
+                gid_map=gid_map,
+                nn_map=nn_map,
+                bias_correct=bias_correct,
             )
 
         except Exception as e:
             out = {}
-            logger.exception('Worker failed for PC: {}'.format(points_control))
+            logger.exception("Worker failed for PC: {}".format(points_control))
             raise e
 
         if scale_outputs:
             # dtype convert in-place so no float data is stored unnecessarily
             for site, site_output in out.items():
                 for k in site_output.keys():
                     # iterate through variable names in each site's output dict
                     if k in cls.OUT_ATTRS:
                         # get dtype and scale for output variable name
-                        dtype = cls.OUT_ATTRS[k].get('dtype', 'float32')
-                        scale_factor = cls.OUT_ATTRS[k].get('scale_factor', 1)
+                        dtype = cls.OUT_ATTRS[k].get("dtype", "float32")
+                        scale_factor = cls.OUT_ATTRS[k].get("scale_factor", 1)
 
                         # apply scale factor and dtype
                         out[site][k] *= scale_factor
 
                         if np.issubdtype(dtype, np.integer):
                             # round after scaling if integer dtype
                             out[site][k] = np.round(out[site][k])
 
                         if isinstance(out[site][k], np.ndarray):
                             # simple astype for arrays
                             out[site][k] = out[site][k].astype(dtype)
                         else:
                             # use numpy array conversion for scalar values
-                            out[site][k] = np.array([out[site][k]],
-                                                    dtype=dtype)[0]
+                            out[site][k] = np.array(
+                                [out[site][k]], dtype=dtype
+                            )[0]
 
         return out
 
     def _parse_gid_map(self, gid_map):
         """
         Parameters
         ----------
@@ -697,52 +750,64 @@
             Mapping of unique integer generation gids (keys) to single integer
             resource gids (values). This enables the user to input unique
             generation gids in the project points that map to non-unique
             resource gids.
         """
 
         if isinstance(gid_map, str):
-            if gid_map.endswith('.csv'):
+            if gid_map.endswith(".csv"):
                 gid_map = pd.read_csv(gid_map).to_dict()
-                assert 'gid' in gid_map, 'Need "gid" in gid_map column'
-                assert 'gid_map' in gid_map, 'Need "gid_map" in gid_map column'
-                gid_map = {gid_map['gid'][i]: gid_map['gid_map'][i]
-                           for i in gid_map['gid'].keys()}
+                msg = f"Need {ResourceMetaField.GID} in gid_map column"
+                assert ResourceMetaField.GID in gid_map, msg
+                assert "gid_map" in gid_map, 'Need "gid_map" in gid_map column'
+                gid_map = {
+                    gid_map[ResourceMetaField.GID][i]: gid_map["gid_map"][i]
+                    for i in gid_map[ResourceMetaField.GID].keys()
+                }
 
-            elif gid_map.endswith('.json'):
-                with open(gid_map, 'r') as f:
+            elif gid_map.endswith(".json"):
+                with open(gid_map) as f:
                     gid_map = json.load(f)
 
         if isinstance(gid_map, dict):
             if not self._multi_h5_res:
                 res_cls = Resource
-                kwargs = {'hsds': self._hsds}
+                kwargs = {"hsds": self._hsds}
             else:
                 res_cls = MultiFileResource
                 kwargs = {}
 
             with res_cls(self.res_file, **kwargs) as res:
                 for gen_gid, res_gid in gid_map.items():
-                    msg1 = ('gid_map values must all be int but received '
-                            '{}: {}'.format(gen_gid, res_gid))
-                    msg2 = ('Could not find the gen_gid to res_gid mapping '
-                            '{}: {} in the resource meta data.'
-                            .format(gen_gid, res_gid))
+                    msg1 = (
+                        "gid_map values must all be int but received "
+                        "{}: {}".format(gen_gid, res_gid)
+                    )
+                    msg2 = (
+                        "Could not find the gen_gid to res_gid mapping "
+                        "{}: {} in the resource meta data.".format(
+                            gen_gid, res_gid
+                        )
+                    )
                     assert isinstance(gen_gid, int), msg1
                     assert isinstance(res_gid, int), msg1
                     assert res_gid in res.meta.index.values, msg2
 
                 for gen_gid in self.project_points.sites:
-                    msg3 = ('Could not find the project points gid {} in the '
-                            'gen_gid input of the gid_map.'.format(gen_gid))
+                    msg3 = (
+                        "Could not find the project points gid {} in the "
+                        "gen_gid input of the gid_map.".format(gen_gid)
+                    )
                     assert gen_gid in gid_map, msg3
 
         elif gid_map is not None:
-            msg = ('Could not parse gid_map, must be None, dict, or path to '
-                   'csv or json, but received: {}'.format(gid_map))
+            msg = (
+                "Could not parse gid_map, must be None, dict, or path to "
+                "csv or json, but received: {}".format(gid_map)
+            )
             logger.error(msg)
             raise InputError(msg)
 
         return gid_map
 
     def _parse_nn_map(self):
         """Parse a nearest-neighbor spatial mapping array if lr_res_file is
@@ -754,32 +819,40 @@
         nn_map : np.ndarray
             Optional 1D array of nearest neighbor mappings associated with the
             res_file to lr_res_file spatial mapping. For details on this
             argument, see the rex.MultiResolutionResource docstring.
         """
         nn_map = None
         if self.lr_res_file is not None:
-
             handler_class = Resource
-            if '*' in self.res_file or '*' in self.lr_res_file:
+            if "*" in self.res_file or "*" in self.lr_res_file:
                 handler_class = MultiFileResource
 
-            with handler_class(self.res_file) as hr_res:
-                with handler_class(self.lr_res_file) as lr_res:
-                    logger.info('Making nearest neighbor map for multi '
-                                'resolution resource data...')
-                    nn_d, nn_map = MultiResolutionResource.make_nn_map(hr_res,
-                                                                       lr_res)
-                    logger.info('Done making nearest neighbor map for multi '
-                                'resolution resource data!')
-
-            logger.info('Made nearest neighbor mapping between nominal-'
-                        'resolution and low-resolution resource files. '
-                        'Min / mean / max dist: {:.3f} / {:.3f} / {:.3f}'
-                        .format(nn_d.min(), nn_d.mean(), nn_d.max()))
+            with handler_class(self.res_file) as hr_res, handler_class(
+                self.lr_res_file
+            ) as lr_res:
+                logger.info(
+                    "Making nearest neighbor map for multi "
+                    "resolution resource data..."
+                )
+                nn_d, nn_map = MultiResolutionResource.make_nn_map(
+                    hr_res, lr_res
+                )
+                logger.info(
+                    "Done making nearest neighbor map for multi "
+                    "resolution resource data!"
+                )
+
+            logger.info(
+                "Made nearest neighbor mapping between nominal-"
+                "resolution and low-resolution resource files. "
+                "Min / mean / max dist: {:.3f} / {:.3f} / {:.3f}".format(
+                    nn_d.min(), nn_d.mean(), nn_d.max()
+                )
+            )
 
         return nn_map
 
     @staticmethod
     def _parse_bc(bias_correct):
         """Parse the bias correction data.
 
@@ -825,31 +898,42 @@
             ``bias_correct`` table on a site-by-site basis. If ``None``, no
             corrections are applied. By default, ``None``.
         """
 
         if isinstance(bias_correct, type(None)):
             return bias_correct
 
-        elif isinstance(bias_correct, str):
-            bias_correct = pd.read_csv(bias_correct)
+        if isinstance(bias_correct, str):
+            bias_correct = pd.read_csv(bias_correct).rename(
+                SupplyCurveField.map_to(ResourceMetaField), axis=1
+            )
 
-        msg = ('Bias correction data must be a filepath to csv or a dataframe '
-               'but received: {}'.format(type(bias_correct)))
+        msg = (
+            "Bias correction data must be a filepath to csv or a dataframe "
+            "but received: {}".format(type(bias_correct))
+        )
         assert isinstance(bias_correct, pd.DataFrame), msg
 
-        msg = ('Bias correction table must have "gid" column but only found: '
-               '{}'.format(list(bias_correct.columns)))
-        assert 'gid' in bias_correct or bias_correct.index.name == 'gid', msg
-
-        if bias_correct.index.name != 'gid':
-            bias_correct = bias_correct.set_index('gid')
-
-        msg = ('Bias correction table must have "method" column but only '
-               'found: {}'.format(list(bias_correct.columns)))
-        assert 'method' in bias_correct, msg
+        msg = (
+            "Bias correction table must have {!r} column but only found: "
+            "{}".format(ResourceMetaField.GID, list(bias_correct.columns))
+        )
+        assert (
+            ResourceMetaField.GID in bias_correct
+            or bias_correct.index.name == ResourceMetaField.GID
+        ), msg
+
+        if bias_correct.index.name != ResourceMetaField.GID:
+            bias_correct = bias_correct.set_index(ResourceMetaField.GID)
+
+        msg = (
+            'Bias correction table must have "method" column but only '
+            "found: {}".format(list(bias_correct.columns))
+        )
+        assert "method" in bias_correct, msg
 
         return bias_correct
 
     def _parse_output_request(self, req):
         """Set the output variables requested from generation.
 
         Parameters
@@ -862,21 +946,23 @@
         output_request : list
             Output variables requested from SAM.
         """
 
         output_request = self._output_request_type_check(req)
 
         # ensure that cf_mean is requested from output
-        if 'cf_mean' not in output_request:
-            output_request.append('cf_mean')
+        if "cf_mean" not in output_request:
+            output_request.append("cf_mean")
 
         for request in output_request:
             if request not in self.OUT_ATTRS:
-                msg = ('User output request "{}" not recognized. '
-                       'Will attempt to extract from PySAM.'.format(request))
+                msg = (
+                    'User output request "{}" not recognized. '
+                    "Will attempt to extract from PySAM.".format(request)
+                )
                 logger.debug(msg)
 
         return list(set(output_request))
 
     def _reduce_kwargs(self, pc, **kwargs):
         """Reduce the global kwargs on a per-worker basis to reduce memory
         footprint
@@ -892,28 +978,27 @@
         Returns
         -------
         kwargs : dict
             Same as input but reduced just for the gids in pc
         """
 
         gids = pc.project_points.gids
-        gid_map = kwargs.get('gid_map', None)
-        bias_correct = kwargs.get('bias_correct', None)
+        gid_map = kwargs.get("gid_map", None)
+        bias_correct = kwargs.get("bias_correct", None)
 
         if bias_correct is not None:
             if gid_map is not None:
                 gids = [gid_map[gid] for gid in gids]
 
             mask = bias_correct.index.isin(gids)
-            kwargs['bias_correct'] = bias_correct[mask]
+            kwargs["bias_correct"] = bias_correct[mask]
 
         return kwargs
 
-    def run(self, out_fpath=None, max_workers=1, timeout=1800,
-            pool_size=None):
+    def run(self, out_fpath=None, max_workers=1, timeout=1800, pool_size=None):
         """Execute a parallel reV generation run with smart data flushing.
 
         Parameters
         ----------
         out_fpath : str, optional
             Path to output file. If ``None``, no output file will
             be written. If the filepath is specified but the module name
@@ -943,49 +1028,72 @@
         # initialize output file
         self._init_fpath(out_fpath, module=ModuleName.GENERATION)
         self._init_h5()
         self._init_out_arrays()
         if pool_size is None:
             pool_size = os.cpu_count() * 2
 
-        kwargs = {'tech': self.tech,
-                  'res_file': self.res_file,
-                  'lr_res_file': self.lr_res_file,
-                  'output_request': self.output_request,
-                  'scale_outputs': self.scale_outputs,
-                  'gid_map': self._gid_map,
-                  'nn_map': self._nn_map,
-                  'bias_correct': self._bc}
-
-        logger.info('Running reV generation for: {}'
-                    .format(self.points_control))
-        logger.debug('The following project points were specified: "{}"'
-                     .format(self.project_points))
-        logger.debug('The following SAM configs are available to this run:\n{}'
-                     .format(pprint.pformat(self.sam_configs, indent=4)))
-        logger.debug('The SAM output variables have been requested:\n{}'
-                     .format(self.output_request))
+        kwargs = {
+            "tech": self.tech,
+            "res_file": self.res_file,
+            "lr_res_file": self.lr_res_file,
+            "output_request": self.output_request,
+            "scale_outputs": self.scale_outputs,
+            "gid_map": self._gid_map,
+            "nn_map": self._nn_map,
+            "bias_correct": self._bc,
+        }
+
+        logger.info(
+            "Running reV generation for: {}".format(self.points_control)
+        )
+        logger.debug(
+            'The following project points were specified: "{}"'.format(
+                self.project_points
+            )
+        )
+        logger.debug(
+            "The following SAM configs are available to this run:\n{}".format(
+                pprint.pformat(self.sam_configs, indent=4)
+            )
+        )
+        logger.debug(
+            "The SAM output variables have been requested:\n{}".format(
+                self.output_request
+            )
+        )
 
         # use serial or parallel execution control based on max_workers
         try:
             if max_workers == 1:
-                logger.debug('Running serial generation for: {}'
-                             .format(self.points_control))
+                logger.debug(
+                    "Running serial generation for: {}".format(
+                        self.points_control
+                    )
+                )
                 for i, pc_sub in enumerate(self.points_control):
                     self.out = self._run_single_worker(pc_sub, **kwargs)
-                    logger.info('Finished reV gen serial compute for: {} '
-                                '(iteration {} out of {})'
-                                .format(pc_sub, i + 1,
-                                        len(self.points_control)))
+                    logger.info(
+                        "Finished reV gen serial compute for: {} "
+                        "(iteration {} out of {})".format(
+                            pc_sub, i + 1, len(self.points_control)
+                        )
+                    )
                 self.flush()
             else:
-                logger.debug('Running parallel generation for: {}'
-                             .format(self.points_control))
-                self._parallel_run(max_workers=max_workers,
-                                   pool_size=pool_size, timeout=timeout,
-                                   **kwargs)
+                logger.debug(
+                    "Running parallel generation for: {}".format(
+                        self.points_control
+                    )
+                )
+                self._parallel_run(
+                    max_workers=max_workers,
+                    pool_size=pool_size,
+                    timeout=timeout,
+                    **kwargs,
+                )
 
         except Exception as e:
-            logger.exception('reV generation failed!')
+            logger.exception("reV generation failed!")
             raise e
 
         return self._out_fpath
```

### Comparing `NREL-reV-0.8.7/reV/handlers/cli_collect.py` & `NREL-reV-0.8.9/reV/handlers/cli_collect.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/handlers/cli_multi_year.py` & `NREL-reV-0.8.9/reV/handlers/cli_multi_year.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/handlers/exclusions.py` & `NREL-reV-0.8.9/reV/handlers/exclusions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 Exclusion layers handler
 """
-import logging
 import json
+import logging
+
 import numpy as np
+from rex.multi_file_resource import MultiFileResource
+from rex.resource import Resource
+from rex.utilities.parse_keys import parse_keys
 
 from reV.utilities.exceptions import HandlerKeyError, MultiFileExclusionError
 
-from rex.utilities.parse_keys import parse_keys
-from rex.resource import Resource
-from rex.multi_file_resource import MultiFileResource
-
 logger = logging.getLogger(__name__)
+LATITUDE, LONGITUDE = "latitude", "longitude"
 
 
 class ExclusionLayers:
     """
     Handler of .h5 file and techmap for Exclusion Layers
     """
 
@@ -77,16 +78,16 @@
         return out
 
     def __contains__(self, layer):
         return layer in self.layers
 
     def _preflight_multi_file(self):
         """Run simple multi-file exclusion checks."""
-        lat_shape = self.h5.shapes['latitude']
-        lon_shape = self.h5.shapes['longitude']
+        lat_shape = self.h5.shapes[LATITUDE]
+        lon_shape = self.h5.shapes[LONGITUDE]
         for layer in self.layers:
             lshape = self.h5.shapes[layer]
             lshape = lshape[1:] if len(lshape) > 2 else lshape
             if lshape != lon_shape or lshape != lat_shape:
                 msg = ('Shape of layer "{}" is {} which does not match '
                        'latitude and longitude shapes of {} and {}. '
                        'Check your exclusion file inputs: {}'
@@ -227,15 +228,15 @@
 
         Returns
         -------
         shape : tuple
         """
         shape = self.h5.attrs.get('shape', None)
         if shape is None:
-            shape = self.h5.shapes['latitude']
+            shape = self.h5.shapes[LATITUDE]
 
         return tuple(shape)
 
     @property
     def chunks(self):
         """
         Exclusion layers chunks default chunk size
@@ -243,39 +244,39 @@
         Returns
         -------
         chunks : tuple | None
             Chunk size of exclusion layers
         """
         chunks = self.h5.attrs.get('chunks', None)
         if chunks is None:
-            chunks = self.h5.chunks['latitude']
+            chunks = self.h5.chunks[LATITUDE]
 
         return chunks
 
     @property
     def latitude(self):
         """
         Latitude coordinates array
 
         Returns
         -------
         ndarray
         """
-        return self['latitude']
+        return self[LATITUDE]
 
     @property
     def longitude(self):
         """
         Longitude coordinates array
 
         Returns
         -------
         ndarray
         """
-        return self['longitude']
+        return self[LONGITUDE]
 
     def get_layer_profile(self, layer):
         """
         Get profile for a specific exclusion layer
 
         Parameters
         ----------
@@ -380,21 +381,21 @@
             Pandas slicing describing which sites and columns to extract
 
         Returns
         -------
         lat : ndarray
             Latitude coordinates
         """
-        if 'latitude' not in self.h5:
+        if LATITUDE not in self.h5:
             msg = ('"latitude" is missing from {}'
                    .format(self.h5_file))
             logger.error(msg)
             raise HandlerKeyError(msg)
 
-        ds_slice = ('latitude', ) + ds_slice
+        ds_slice = (LATITUDE, ) + ds_slice
 
         lat = self.h5[ds_slice]
 
         return lat
 
     def _get_longitude(self, *ds_slice):
         """
@@ -406,21 +407,21 @@
             Pandas slicing describing which sites and columns to extract
 
         Returns
         -------
         lon : ndarray
             Longitude coordinates
         """
-        if 'longitude' not in self.h5:
+        if LONGITUDE not in self.h5:
             msg = ('"longitude" is missing from {}'
                    .format(self.h5_file))
             logger.error(msg)
             raise HandlerKeyError(msg)
 
-        ds_slice = ('longitude', ) + ds_slice
+        ds_slice = (LONGITUDE, ) + ds_slice
 
         lon = self.h5[ds_slice]
 
         return lon
 
     def _get_layer(self, layer_name, *ds_slice):
         """
```

### Comparing `NREL-reV-0.8.7/reV/handlers/multi_year.py` & `NREL-reV-0.8.9/reV/handlers/multi_year.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: utf-8 -*-
 """
 Classes to collect reV outputs from multiple annual files.
 """
 import glob
-import time
 import logging
-import numpy as np
 import os
-import pandas as pd
+import time
 from warnings import warn
 
-from rex import Resource
-from rex.utilities.utilities import (get_class_properties, parse_year,
-                                     get_lat_lon_cols)
+import numpy as np
+import pandas as pd
 from gaps.pipeline import parse_previous_status
+from rex import Resource
+from rex.utilities.utilities import (
+    get_class_properties,
+    get_lat_lon_cols,
+    parse_year,
+)
 
-from reV.handlers.outputs import Outputs
 from reV.config.output_request import SAMOutputRequest
-from reV.utilities.exceptions import HandlerRuntimeError, ConfigError
-from reV.utilities import log_versions, ModuleName
+from reV.handlers.outputs import Outputs
+from reV.utilities import ModuleName, log_versions
+from reV.utilities.exceptions import ConfigError, HandlerRuntimeError
 
 logger = logging.getLogger(__name__)
 
 
 class MultiYearGroup:
     """
     Handle group parameters
```

### Comparing `NREL-reV-0.8.7/reV/handlers/outputs.py` & `NREL-reV-0.8.9/reV/handlers/outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 Classes to handle reV h5 output files.
 """
+import json
 import logging
+import sys
+
 import NRWAL
 import PySAM
 import rex
-import sys
-import json
+from rex.outputs import Outputs as rexOutputs
 
 from reV.version import __version__
-from rex.outputs import Outputs as rexOutputs
 
 logger = logging.getLogger(__name__)
 
 
 class Outputs(rexOutputs):
     """
     Base class to handle reV output data in .h5 format
@@ -24,16 +25,16 @@
     The reV Outputs handler can be used to initialize h5 files in the standard
     reV/rex resource data format.
 
     >>> from reV import Outputs
     >>> import pandas as pd
     >>> import numpy as np
     >>>
-    >>> meta = pd.DataFrame({'latitude': np.ones(100),
-    >>>                      'longitude': np.ones(100)})
+    >>> meta = pd.DataFrame({SupplyCurveField.LATITUDE: np.ones(100),
+    >>>                      SupplyCurveField.LONGITUDE: np.ones(100)})
     >>>
     >>> time_index = pd.date_range('20210101', '20220101', freq='1h',
     >>>                            closed='right')
     >>>
     >>> with Outputs('test.h5', 'w') as f:
     >>>     f.meta = meta
     >>>     f.time_index = time_index
```

### Comparing `NREL-reV-0.8.7/reV/handlers/transmission.py` & `NREL-reV-0.8.9/reV/handlers/transmission.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/hybrids/cli_hybrids.py` & `NREL-reV-0.8.9/reV/hybrids/cli_hybrids.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/hybrids/hybrids.py` & `NREL-reV-0.8.9/reV/hybrids/hybrids.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 # -*- coding: utf-8 -*-
 """reV Hybridization module.
 
 @author: ppinchuk
 """
+
 import logging
-import numpy as np
 import re
-import pandas as pd
+from collections import namedtuple
 from string import ascii_letters
 from warnings import warn
-from collections import namedtuple
-
-from reV.handlers.outputs import Outputs
-from reV.utilities.exceptions import (FileInputError, InputError,
-                                      InputWarning, OutputWarning)
-from reV.hybrids.hybrid_methods import HYBRID_METHODS
 
+import numpy as np
+import pandas as pd
 from rex.resource import Resource
 from rex.utilities.utilities import to_records_array
 
+from reV.handlers.outputs import Outputs
+from reV.hybrids.hybrid_methods import HYBRID_METHODS
+from reV.utilities import SupplyCurveField
+from reV.utilities.exceptions import (
+    FileInputError,
+    InputError,
+    InputWarning,
+    OutputWarning,
+)
+
 logger = logging.getLogger(__name__)
 
-MERGE_COLUMN = 'sc_point_gid'
+MERGE_COLUMN = SupplyCurveField.SC_POINT_GID
 PROFILE_DSET_REGEX = 'rep_profiles_[0-9]+$'
 SOLAR_PREFIX = 'solar_'
 WIND_PREFIX = 'wind_'
 NON_DUPLICATE_COLS = {
-    'latitude', 'longitude', 'country', 'state', 'county', 'elevation',
-    'timezone', 'sc_point_gid', 'sc_row_ind', 'sc_col_ind'
+    SupplyCurveField.LATITUDE, SupplyCurveField.LONGITUDE,
+    SupplyCurveField.COUNTRY, SupplyCurveField.STATE, SupplyCurveField.COUNTY,
+    SupplyCurveField.ELEVATION, SupplyCurveField.TIMEZONE,
+    SupplyCurveField.SC_POINT_GID, SupplyCurveField.SC_ROW_IND,
+    SupplyCurveField.SC_COL_IND
 }
-DROPPED_COLUMNS = ['gid']
-DEFAULT_FILL_VALUES = {'solar_capacity': 0, 'wind_capacity': 0,
-                       'solar_mean_cf': 0, 'wind_mean_cf': 0}
+DROPPED_COLUMNS = [SupplyCurveField.GID]
+DEFAULT_FILL_VALUES = {f'solar_{SupplyCurveField.CAPACITY}': 0,
+                       f'wind_{SupplyCurveField.CAPACITY}': 0,
+                       f'solar_{SupplyCurveField.MEAN_CF}': 0,
+                       f'wind_{SupplyCurveField.MEAN_CF}': 0}
 OUTPUT_PROFILE_NAMES = ['hybrid_profile',
                         'hybrid_solar_profile',
                         'hybrid_wind_profile']
 RatioColumns = namedtuple('RatioColumns', ['num', 'denom', 'fixed'],
                           defaults=(None, None, None))
 
 
 class ColNameFormatter:
-    """Column name formatting helper class. """
+    """Column name formatting helper class."""
+
     ALLOWED = set(ascii_letters)
 
     @classmethod
     def fmt(cls, n):
         """Format an input column name to remove excess chars and whitespace.
 
         This method should help facilitate the merging of column names
@@ -57,19 +69,19 @@
 
         Returns
         -------
         str
             The column name with all characters except ascii stripped
             and all lowercase.
         """
-        return ''.join(c for c in n if c in cls.ALLOWED).lower()
+        return "".join(c for c in n if c in cls.ALLOWED).lower()
 
 
 class HybridsData:
-    """Hybrids input data container. """
+    """Hybrids input data container."""
 
     def __init__(self, solar_fpath, wind_fpath):
         """
         Parameters
         ----------
         solar_fpath : str
             Filepath to rep profile output file to extract solar profiles and
@@ -154,15 +166,16 @@
         Returns
         -------
         hybrid_time_index : pd.datetimeindex
             Time index for the hybrid rep profiles.
         """
         if self._hybrid_time_index is None:
             self._hybrid_time_index = self.solar_time_index.join(
-                self.wind_time_index, how='inner')
+                self.wind_time_index, how="inner"
+            )
         return self._hybrid_time_index
 
     def contains_col(self, col_name):
         """Check if input column name exists in either meta data set.
 
         Parameters
         ----------
@@ -198,17 +211,19 @@
 
         Raises
         ------
         FileInputError
             If len(time_index) < 8760 for the hybrid profile.
         """
         if len(self.hybrid_time_index) < 8760:
-            msg = ("The length of the merged time index ({}) is less than "
-                   "8760. Please ensure that the input profiles have a "
-                   "time index that overlaps >= 8760 times.")
+            msg = (
+                "The length of the merged time index ({}) is less than "
+                "8760. Please ensure that the input profiles have a "
+                "time index that overlaps >= 8760 times."
+            )
             e = msg.format(len(self.hybrid_time_index))
             logger.error(e)
             raise FileInputError(e)
 
     def _validate_num_profiles(self):
         """Validate the number of input profiles.
 
@@ -216,75 +231,83 @@
         ------
         FileInputError
             If # of rep_profiles > 1.
         """
         for fp in [self.solar_fpath, self.wind_fpath]:
             with Resource(fp) as res:
                 profile_dset_names = [
-                    n for n in res.dsets
-                    if self.__profile_reg_check.match(n)
+                    n for n in res.dsets if self.__profile_reg_check.match(n)
                 ]
                 if not profile_dset_names:
-                    msg = ("Did not find any data sets matching the regex: "
-                           "{!r} in {!r}. Please ensure that the profile data "
-                           "exists and that the data set is named correctly.")
+                    msg = (
+                        "Did not find any data sets matching the regex: "
+                        "{!r} in {!r}. Please ensure that the profile data "
+                        "exists and that the data set is named correctly."
+                    )
                     e = msg.format(PROFILE_DSET_REGEX, fp)
                     logger.error(e)
                     raise FileInputError(e)
-                elif len(profile_dset_names) > 1:
+                if len(profile_dset_names) > 1:
                     msg = ("Found more than one profile in {!r}: {}. "
                            "This module is not intended for hybridization of "
                            "multiple representative profiles. Please re-run "
                            "on a single aggregated profile.")
                     e = msg.format(fp, profile_dset_names)
                     logger.error(e)
                     raise FileInputError(e)
-                else:
-                    self.profile_dset_names += profile_dset_names
+                self.profile_dset_names += profile_dset_names
 
     def _validate_merge_col_exists(self):
         """Validate the existence of the merge column.
 
         Raises
         ------
         FileInputError
             If merge column is missing from either the solar or
             the wind meta data.
         """
-        msg = ("Cannot hybridize: merge column {!r} missing from the "
-               "{} meta data! ({!r})")
+        msg = (
+            "Cannot hybridize: merge column {!r} missing from the "
+            "{} meta data! ({!r})"
+        )
 
         mc = ColNameFormatter.fmt(MERGE_COLUMN)
-        for cols, fp, res in zip([self.__solar_cols, self.__wind_cols],
-                                 [self.solar_fpath, self.wind_fpath],
-                                 ['solar', 'wind']):
+        for cols, fp, res in zip(
+            [self.__solar_cols, self.__wind_cols],
+            [self.solar_fpath, self.wind_fpath],
+            ["solar", "wind"],
+        ):
             if mc not in cols:
                 e = msg.format(MERGE_COLUMN, res, fp)
                 logger.error(e)
                 raise FileInputError(e)
 
     def _validate_unique_merge_col(self):
         """Validate the existence of unique values in the merge column.
 
         Raises
         ------
         FileInputError
             If merge column contains duplicate values  in either the solar or
             the wind meta data.
         """
-        msg = ("Duplicate {}s were found. This is likely due to resource "
-               "class binning, which is not supported at this time. "
-               "Please re-run supply curve aggregation without "
-               "resource class binning and ensure there are no duplicate "
-               "values in {!r}. File: {!r}")
+        msg = (
+            "Duplicate {}s were found. This is likely due to resource "
+            "class binning, which is not supported at this time. "
+            "Please re-run supply curve aggregation without "
+            "resource class binning and ensure there are no duplicate "
+            "values in {!r}. File: {!r}"
+        )
 
         mc = ColNameFormatter.fmt(MERGE_COLUMN)
-        for ds, cols, fp in zip([self.solar_meta, self.wind_meta],
-                                [self.__solar_cols, self.__wind_cols],
-                                [self.solar_fpath, self.wind_fpath]):
+        for ds, cols, fp in zip(
+            [self.solar_meta, self.wind_meta],
+            [self.__solar_cols, self.__wind_cols],
+            [self.solar_fpath, self.wind_fpath],
+        ):
             merge_col = ds.columns[cols == mc].item()
             if not ds[merge_col].is_unique:
                 e = msg.format(merge_col, merge_col, fp)
                 logger.error(e)
                 raise FileInputError(e)
 
     def _validate_merge_col_overlaps(self):
@@ -299,32 +322,41 @@
         merge_col = self.solar_meta.columns[self.__solar_cols == mc].item()
         solar_vals = set(self.solar_meta[merge_col].values)
         merge_col = self.wind_meta.columns[self.__wind_cols == mc].item()
         wind_vals = set(self.wind_meta[merge_col].values)
         self.merge_col_overlap_values = solar_vals & wind_vals
 
         if not self.merge_col_overlap_values:
-            msg = ("No overlap detected in the values of {!r} across the "
-                   "input files. Please ensure that at least one of the "
-                   "{!r} values is the same for input files {!r} and {!r}")
-            e = msg.format(merge_col, merge_col, self.solar_fpath,
-                           self.wind_fpath)
+            msg = (
+                "No overlap detected in the values of {!r} across the "
+                "input files. Please ensure that at least one of the "
+                "{!r} values is the same for input files {!r} and {!r}"
+            )
+            e = msg.format(
+                merge_col, merge_col, self.solar_fpath, self.wind_fpath
+            )
             logger.error(e)
             raise FileInputError(e)
 
 
 class MetaHybridizer:
     """Framework to handle hybridization of meta data."""
 
-    _INTERNAL_COL_PREFIX = '_h_internal'
+    _INTERNAL_COL_PREFIX = "_h_internal"
 
-    def __init__(self, data, allow_solar_only=False,
-                 allow_wind_only=False, fillna=None,
-                 limits=None, ratio_bounds=None,
-                 ratio='solar_capacity/wind_capacity'):
+    def __init__(
+        self,
+        data,
+        allow_solar_only=False,
+        allow_wind_only=False,
+        fillna=None,
+        limits=None,
+        ratio_bounds=None,
+        ratio="solar_capacity/wind_capacity",
+    ):
         """
         Parameters
         ----------
         data : `HybridsData`
             Instance of `HybridsData` containing input data to
             hybridize.
         allow_solar_only : bool, optional
@@ -379,31 +411,30 @@
         self._fillna = {**DEFAULT_FILL_VALUES, **(fillna or {})}
         self._limits = limits or {}
         self._ratio_bounds = ratio_bounds
         self._ratio = ratio
         self._hybrid_meta = None
         self.__hybrid_meta_cols = None
         self.__col_name_map = None
-        self.__solar_rpi_n = '{}_solar_rpidx'.format(self._INTERNAL_COL_PREFIX)
-        self.__wind_rpi_n = '{}_wind_rpidx'.format(self._INTERNAL_COL_PREFIX)
+        self.__solar_rpi_n = "{}_solar_rpidx".format(self._INTERNAL_COL_PREFIX)
+        self.__wind_rpi_n = "{}_wind_rpidx".format(self._INTERNAL_COL_PREFIX)
 
     @property
     def hybrid_meta(self):
         """Hybridized summary for the representative profiles.
 
         Returns
         -------
         hybrid_meta : pd.DataFrame
             Summary for the hybridized representative profiles.
             At the very least, this has a column that the data was merged on.
         """
         if self._hybrid_meta is None or self.__hybrid_meta_cols is None:
             return self._hybrid_meta
-        else:
-            return self._hybrid_meta[self.__hybrid_meta_cols]
+        return self._hybrid_meta[self.__hybrid_meta_cols]
 
     def validate_input(self):
         """Validate the input parameters.
 
         This method validates that the input limit, fill, and ratio columns
         are formatted correctly.
         """
@@ -422,26 +453,28 @@
         Raises
         ------
         InputError
             If limits columns are not prefixed correctly.
         """
         for col in self._limits:
             self.__validate_col_prefix(
-                col, (SOLAR_PREFIX, WIND_PREFIX), input_name='limits'
+                col, (SOLAR_PREFIX, WIND_PREFIX), input_name="limits"
             )
 
     @staticmethod
     def __validate_col_prefix(col, prefixes, input_name):
-        """Validate the the col starts with the correct prefix. """
+        """Validate the the col starts with the correct prefix."""
 
         missing = [not col.startswith(p) for p in prefixes]
         if all(missing):
-            msg = ("Input {0} column {1!r} does not start with a valid "
-                   "prefix: {2!r}. Please ensure that the {0} column "
-                   "names specify the correct resource prefix.")
+            msg = (
+                "Input {0} column {1!r} does not start with a valid "
+                "prefix: {2!r}. Please ensure that the {0} column "
+                "names specify the correct resource prefix."
+            )
             e = msg.format(input_name, col, prefixes)
             logger.error(e)
             raise InputError(e)
 
     def _validate_fillna_cols_prefixed(self):
         """Ensure the fillna columns are formatted correctly.
 
@@ -453,15 +486,15 @@
         Raises
         ------
         InputError
             If fillna columns are not prefixed correctly.
         """
         for col in self._fillna:
             self.__validate_col_prefix(
-                col, (SOLAR_PREFIX, WIND_PREFIX), input_name='fillna'
+                col, (SOLAR_PREFIX, WIND_PREFIX), input_name="fillna"
             )
 
     def _validate_ratio_input(self):
         """Validate the ratio input parameters.
 
         This method validates that the input ratio columns are formatted
         correctly and exist in the input data. It also verifies that
@@ -483,68 +516,78 @@
         ------
         InputError
             If ratio is not a len 2 container of floats.
         """
 
         try:
             if len(self._ratio_bounds) != 2:
-                msg = ("Length of input for ratio_bounds is {} - but is "
-                       "required to be of length 2. Please make sure this "
-                       "input is a len 2 container of floats. If you would "
-                       "like to specify a single ratio value, use the same "
-                       "float for both limits (i.e. ratio_bounds=(1, 1)).")
+                msg = (
+                    "Length of input for ratio_bounds is {} - but is "
+                    "required to be of length 2. Please make sure this "
+                    "input is a len 2 container of floats. If you would "
+                    "like to specify a single ratio value, use the same "
+                    "float for both limits (i.e. ratio_bounds=(1, 1))."
+                )
                 e = msg.format(len(self._ratio_bounds))
                 logger.error(e)
                 raise InputError(e)
         except TypeError:
-            msg = ("Input for ratio_bounds not understood: {!r}. "
-                   "Please make sure this value is a len 2 container "
-                   "of floats.")
+            msg = (
+                "Input for ratio_bounds not understood: {!r}. "
+                "Please make sure this value is a len 2 container "
+                "of floats."
+            )
             e = msg.format(self._ratio_bounds)
             logger.error(e)
             raise InputError(e) from None
 
     def _validate_ratio_type(self):
         """Ensure that the ratio input is a string.
 
         Raises
         ------
         InputError
             If `ratio` is not a string.
         """
         if not isinstance(self._ratio, str):
-            msg = ("Ratio input type {} not understood. Please make sure "
-                   "the ratio input is a string in the form "
-                   "'numerator_column_name/denominator_column_name'. Ratio "
-                   "input: {!r}")
+            msg = (
+                "Ratio input type {} not understood. Please make sure "
+                "the ratio input is a string in the form "
+                "'numerator_column_name/denominator_column_name'. Ratio "
+                "input: {!r}"
+            )
             e = msg.format(type(self._ratio), self._ratio)
             logger.error(e)
             raise InputError(e)
 
     def _validate_ratio_format(self):
         """Validate that the ratio input format is correct and can be parsed.
 
         Raises
         ------
         InputError
             If the '/' character is missing or of there are too many
             '/' characters.
         """
-        if '/' not in self._ratio:
-            msg = ("Ratio input {} does not contain the '/' character. "
-                   "Please make sure the ratio input is a string in the form "
-                   "'numerator_column_name/denominator_column_name'")
+        if "/" not in self._ratio:
+            msg = (
+                "Ratio input {} does not contain the '/' character. "
+                "Please make sure the ratio input is a string in the form "
+                "'numerator_column_name/denominator_column_name'"
+            )
             e = msg.format(self._ratio)
             logger.error(e)
             raise InputError(e)
 
         if len(self._ratio_cols) != 2:
-            msg = ("Ratio input {} contains too many '/' characters. Please "
-                   "make sure the ratio input is a string in the form "
-                   "'numerator_column_name/denominator_column_name'.")
+            msg = (
+                "Ratio input {} contains too many '/' characters. Please "
+                "make sure the ratio input is a string in the form "
+                "'numerator_column_name/denominator_column_name'."
+            )
             e = msg.format(self._ratio)
             logger.error(e)
             raise InputError(e)
 
     def _validate_ratio_cols_prefixed(self):
         """Ensure the ratio columns are formatted correctly.
 
@@ -557,203 +600,218 @@
         ------
         InputError
             If ratio columns are not prefixed correctly.
         """
 
         for col in self._ratio_cols:
             self.__validate_col_prefix(
-                col, (SOLAR_PREFIX, WIND_PREFIX), input_name='ratios'
+                col, (SOLAR_PREFIX, WIND_PREFIX), input_name="ratios"
             )
 
     def _validate_ratio_cols_exist(self):
         """Ensure the ratio columns exist if a ratio is specified.
 
         Raises
         ------
         FileInputError
             If ratio columns are not found in the meta data.
         """
 
         for col in self._ratio_cols:
-            no_prefix_name = "_".join(col.split('_')[1:])
+            no_prefix_name = "_".join(col.split("_")[1:])
             if not self.data.contains_col(no_prefix_name):
-                msg = ("Input ratios column {!r} not found in either meta "
-                       "data! Please check the input files {!r} and {!r}")
-                e = msg.format(no_prefix_name, self.data.solar_fpath,
-                               self.data.wind_fpath)
+                msg = (
+                    "Input ratios column {!r} not found in either meta "
+                    "data! Please check the input files {!r} and {!r}"
+                )
+                e = msg.format(
+                    no_prefix_name, self.data.solar_fpath, self.data.wind_fpath
+                )
                 logger.error(e)
                 raise FileInputError(e)
 
     @property
     def _ratio_cols(self):
-        """Get the ratio columns from the ratio input. """
+        """Get the ratio columns from the ratio input."""
         if self._ratio is None:
             return []
-        return self._ratio.strip().split('/')
+        return self._ratio.strip().split("/")
 
     def hybridize(self):
         """Combine the solar and wind metas and run hybridize methods."""
         self._format_meta_pre_merge()
         self._merge_solar_wind_meta()
-        self._verify_lat_long_match_post_merge()
+        self._verify_lat_lon_match_post_merge()
         self._format_meta_post_merge()
         self._fillna_meta_cols()
         self._apply_limits()
         self._limit_by_ratio()
         self._add_hybrid_cols()
         self._sort_hybrid_meta_cols()
 
     def _format_meta_pre_merge(self):
-        """Prepare solar and wind meta for merging. """
+        """Prepare solar and wind meta for merging."""
         self.__col_name_map = {
             ColNameFormatter.fmt(c): c
             for c in self.data.solar_meta.columns.values
         }
 
         self._rename_cols(self.data.solar_meta, prefix=SOLAR_PREFIX)
         self._rename_cols(self.data.wind_meta, prefix=WIND_PREFIX)
 
         self._save_rep_prof_index_internally()
 
     @staticmethod
     def _rename_cols(df, prefix):
-        """Replace column names with the ColNameFormatter.fmt is needed. """
+        """Replace column names with the ColNameFormatter.fmt is needed."""
         df.columns = [
             ColNameFormatter.fmt(col_name)
             if col_name in NON_DUPLICATE_COLS
-            else '{}{}'.format(prefix, col_name)
+            else "{}{}".format(prefix, col_name)
             for col_name in df.columns.values
         ]
 
     def _save_rep_prof_index_internally(self):
-        """Save rep profiles index in hybrid meta for access later. """
+        """Save rep profiles index in hybrid meta for access later."""
 
         self.data.solar_meta[self.__solar_rpi_n] = self.data.solar_meta.index
         self.data.wind_meta[self.__wind_rpi_n] = self.data.wind_meta.index
 
     def _merge_solar_wind_meta(self):
-        """Merge the wind and solar meta DataFrames. """
+        """Merge the wind and solar meta DataFrames."""
         self._hybrid_meta = self.data.solar_meta.merge(
             self.data.wind_meta,
             on=ColNameFormatter.fmt(MERGE_COLUMN),
-            suffixes=[None, '_x'], how=self._merge_type()
+            suffixes=[None, "_x"],
+            how=self._merge_type(),
         )
 
     def _merge_type(self):
-        """Determine the type of merge to use for meta based on user input. """
+        """Determine the type of merge to use for meta based on user input."""
         if self._allow_solar_only and self._allow_wind_only:
             return 'outer'
-        elif self._allow_solar_only and not self._allow_wind_only:
+        if self._allow_solar_only and not self._allow_wind_only:
             return 'left'
-        elif not self._allow_solar_only and self._allow_wind_only:
+        if not self._allow_solar_only and self._allow_wind_only:
             return 'right'
         return 'inner'
 
     def _format_meta_post_merge(self):
-        """Format hybrid meta after merging. """
+        """Format hybrid meta after merging."""
 
         duplicate_cols = [n for n in self._hybrid_meta.columns if "_x" in n]
         self._propagate_duplicate_cols(duplicate_cols)
         self._drop_cols(duplicate_cols)
         self._hybrid_meta.rename(self.__col_name_map, inplace=True, axis=1)
-        self._hybrid_meta.index.name = 'gid'
+        self._hybrid_meta.index.name = SupplyCurveField.GID
 
     def _propagate_duplicate_cols(self, duplicate_cols):
-        """Fill missing column values from outer merge. """
+        """Fill missing column values from outer merge."""
         for duplicate in duplicate_cols:
             no_suffix = "_".join(duplicate.split("_")[:-1])
             null_idx = self._hybrid_meta[no_suffix].isnull()
             non_null_vals = self._hybrid_meta.loc[null_idx, duplicate].values
             self._hybrid_meta.loc[null_idx, no_suffix] = non_null_vals
 
     def _drop_cols(self, duplicate_cols):
-        """Drop any remaning duplicate and 'DROPPED_COLUMNS' columns. """
+        """Drop any remaning duplicate and 'DROPPED_COLUMNS' columns."""
         self._hybrid_meta.drop(
             duplicate_cols + DROPPED_COLUMNS,
-            axis=1, inplace=True, errors='ignore'
+            axis=1,
+            inplace=True,
+            errors="ignore",
         )
 
     def _sort_hybrid_meta_cols(self):
-        """Sort the columns of the hybrid meta. """
+        """Sort the columns of the hybrid meta."""
         self.__hybrid_meta_cols = sorted(
-            [c for c in self._hybrid_meta.columns
-             if not c.startswith(self._INTERNAL_COL_PREFIX)],
-            key=self._column_sorting_key
+            [
+                c
+                for c in self._hybrid_meta.columns
+                if not c.startswith(self._INTERNAL_COL_PREFIX)
+            ],
+            key=self._column_sorting_key,
         )
 
     def _column_sorting_key(self, c):
-        """Helper function to sort hybrid meta columns. """
+        """Helper function to sort hybrid meta columns."""
         first_index = 0
-        if c.startswith('hybrid'):
+        if c.startswith("hybrid"):
             first_index = 1
-        elif c.startswith('solar'):
+        elif c.startswith("solar"):
             first_index = 2
-        elif c.startswith('wind'):
+        elif c.startswith("wind"):
             first_index = 3
         elif c == MERGE_COLUMN:
             first_index = -1
         return first_index, self._hybrid_meta.columns.get_loc(c)
 
-    def _verify_lat_long_match_post_merge(self):
+    def _verify_lat_lon_match_post_merge(self):
         """Verify that all the lat/lon values match post merge."""
-        lat = self._verify_col_match_post_merge(col_name='latitude')
-        lon = self._verify_col_match_post_merge(col_name='longitude')
+        lat = self._verify_col_match_post_merge(
+            col_name=ColNameFormatter.fmt(SupplyCurveField.LATITUDE)
+        )
+        lon = self._verify_col_match_post_merge(
+            col_name=ColNameFormatter.fmt(SupplyCurveField.LONGITUDE)
+        )
         if not lat or not lon:
-            msg = ("Detected mismatched coordinate values (latitude or "
-                   "longitude) post merge. Please ensure that all matching "
-                   "values of {!r} correspond to the same values of latitude "
-                   "and longitude across the input files {!r} and {!r}")
-            e = msg.format(MERGE_COLUMN, self.data.solar_fpath,
-                           self.data.wind_fpath)
+            msg = (
+                "Detected mismatched coordinate values (latitude or "
+                "longitude) post merge. Please ensure that all matching "
+                "values of {!r} correspond to the same values of latitude "
+                "and longitude across the input files {!r} and {!r}"
+            )
+            e = msg.format(
+                MERGE_COLUMN, self.data.solar_fpath, self.data.wind_fpath
+            )
             logger.error(e)
             raise FileInputError(e)
 
     def _verify_col_match_post_merge(self, col_name):
-        """Verify that all (non-null) values in a column match post merge. """
+        """Verify that all (non-null) values in a column match post merge."""
         c1, c2 = col_name, '{}_x'.format(col_name)
         if c1 in self._hybrid_meta.columns and c2 in self._hybrid_meta.columns:
             compare_df = self._hybrid_meta[
                 (self._hybrid_meta[c1].notnull())
                 & (self._hybrid_meta[c2].notnull())
             ]
             return np.allclose(compare_df[c1], compare_df[c2])
-        else:
-            return True
+        return True
 
     def _fillna_meta_cols(self):
-        """Fill N/A values as specified by user (and internals). """
+        """Fill N/A values as specified by user (and internals)."""
         for col_name, fill_value in self._fillna.items():
             if col_name in self._hybrid_meta.columns:
                 self._hybrid_meta[col_name].fillna(fill_value, inplace=True)
             else:
-                self.__warn_missing_col(col_name, action='fill')
+                self.__warn_missing_col(col_name, action="fill")
 
         self._hybrid_meta[self.__solar_rpi_n].fillna(-1, inplace=True)
         self._hybrid_meta[self.__wind_rpi_n].fillna(-1, inplace=True)
 
     @staticmethod
     def __warn_missing_col(col_name, action):
-        """Warn that a column the user request an action for is missing. """
+        """Warn that a column the user request an action for is missing."""
         msg = ("Skipping {} values for {!r}: Unable to find column "
                "in hybrid meta. Did you forget to prefix with "
                "{!r} or {!r}? ")
         w = msg.format(action, col_name, SOLAR_PREFIX, WIND_PREFIX)
         logger.warning(w)
         warn(w, InputWarning)
 
     def _apply_limits(self):
-        """Clip column values as specified by user. """
+        """Clip column values as specified by user."""
         for col_name, max_value in self._limits.items():
             if col_name in self._hybrid_meta.columns:
                 self._hybrid_meta[col_name].clip(upper=max_value, inplace=True)
             else:
-                self.__warn_missing_col(col_name, action='limit')
+                self.__warn_missing_col(col_name, action="limit")
 
     def _limit_by_ratio(self):
-        """ Limit the given pair of ratio columns based on input ratio. """
+        """Limit the given pair of ratio columns based on input ratio."""
 
         if self._ratio_bounds is None:
             return
 
         numerator_col, denominator_col = self._ratio_cols
         min_ratio, max_ratio = sorted(self._ratio_bounds)
 
@@ -761,16 +819,15 @@
             self.data.merge_col_overlap_values
         )
 
         numerator_vals = self._hybrid_meta[numerator_col].copy()
         denominator_vals = self._hybrid_meta[denominator_col].copy()
 
         ratios = (
-            numerator_vals.loc[overlap_idx]
-            / denominator_vals.loc[overlap_idx]
+            numerator_vals.loc[overlap_idx] / denominator_vals.loc[overlap_idx]
         )
         ratio_too_low = (ratios < min_ratio) & overlap_idx
         ratio_too_high = (ratios > max_ratio) & overlap_idx
 
         numerator_vals.loc[ratio_too_high] = (
             denominator_vals.loc[ratio_too_high].values * max_ratio
         )
@@ -780,24 +837,26 @@
 
         h_num_name = "hybrid_{}".format(numerator_col)
         h_denom_name = "hybrid_{}".format(denominator_col)
         self._hybrid_meta[h_num_name] = numerator_vals.values
         self._hybrid_meta[h_denom_name] = denominator_vals.values
 
     def _add_hybrid_cols(self):
-        """Add new hybrid columns using registered hybrid methods. """
+        """Add new hybrid columns using registered hybrid methods."""
         for new_col_name, method in HYBRID_METHODS.items():
             out = method(self)
             if out is not None:
                 try:
                     self._hybrid_meta[new_col_name] = out
                 except ValueError as e:
-                    msg = ("Unable to add {!r} column to hybrid meta. The "
-                           "following exception was raised when adding "
-                           "the data output by '{}': {!r}.")
+                    msg = (
+                        "Unable to add {!r} column to hybrid meta. The "
+                        "following exception was raised when adding "
+                        "the data output by '{}': {!r}."
+                    )
                     w = msg.format(new_col_name, method.__name__, e)
                     logger.warning(w)
                     warn(w, OutputWarning)
 
     @property
     def solar_profile_indices_map(self):
         """Map hybrid to solar rep indices.
@@ -839,17 +898,25 @@
 
         return idxs.index.values, idxs.values
 
 
 class Hybridization:
     """Hybridization"""
 
-    def __init__(self, solar_fpath, wind_fpath, allow_solar_only=False,
-                 allow_wind_only=False, fillna=None, limits=None,
-                 ratio_bounds=None, ratio='solar_capacity/wind_capacity'):
+    def __init__(
+        self,
+        solar_fpath,
+        wind_fpath,
+        allow_solar_only=False,
+        allow_wind_only=False,
+        fillna=None,
+        limits=None,
+        ratio_bounds=None,
+        ratio="solar_capacity/wind_capacity",
+    ):
         """Framework to handle hybridization of SC and corresponding profiles.
 
         ``reV`` hybrids computes a "hybrid" wind and solar supply curve,
         where each supply curve point contains some wind and some solar
         capacity. Various ratio limits on wind-to-solar farm properties
         (e.g. wind-to-solar capacity) can be applied during the
         hybridization process. Hybrid generation profiles are also
@@ -905,42 +972,65 @@
             would limit the ratio of the solar to wind capacities as
             specified by the ``ratio_bounds`` input. If ``ratio_bounds``
             is None, this input does nothing. The names of the columns
             should be prefixed with one of the prefixes defined as class
             variables. By default ``'solar_capacity/wind_capacity'``.
         """
 
-        logger.info('Running hybridization of rep profiles with solar_fpath: '
-                    '"{}"'.format(solar_fpath))
-        logger.info('Running hybridization of rep profiles with solar_fpath: '
-                    '"{}"'.format(wind_fpath))
-        logger.info('Running hybridization of rep profiles with '
-                    'allow_solar_only: "{}"'.format(allow_solar_only))
-        logger.info('Running hybridization of rep profiles with '
-                    'allow_wind_only: "{}"'.format(allow_wind_only))
-        logger.info('Running hybridization of rep profiles with fillna: "{}"'
-                    .format(fillna))
-        logger.info('Running hybridization of rep profiles with limits: "{}"'
-                    .format(limits))
-        logger.info('Running hybridization of rep profiles with ratio_bounds: '
-                    '"{}"'.format(ratio_bounds))
-        logger.info('Running hybridization of rep profiles with ratio: "{}"'
-                    .format(ratio))
+        logger.info(
+            "Running hybridization of rep profiles with solar_fpath: "
+            '"{}"'.format(solar_fpath)
+        )
+        logger.info(
+            "Running hybridization of rep profiles with solar_fpath: "
+            '"{}"'.format(wind_fpath)
+        )
+        logger.info(
+            "Running hybridization of rep profiles with "
+            'allow_solar_only: "{}"'.format(allow_solar_only)
+        )
+        logger.info(
+            "Running hybridization of rep profiles with "
+            'allow_wind_only: "{}"'.format(allow_wind_only)
+        )
+        logger.info(
+            'Running hybridization of rep profiles with fillna: "{}"'.format(
+                fillna
+            )
+        )
+        logger.info(
+            'Running hybridization of rep profiles with limits: "{}"'.format(
+                limits
+            )
+        )
+        logger.info(
+            "Running hybridization of rep profiles with ratio_bounds: "
+            '"{}"'.format(ratio_bounds)
+        )
+        logger.info(
+            'Running hybridization of rep profiles with ratio: "{}"'.format(
+                ratio
+            )
+        )
 
         self.data = HybridsData(solar_fpath, wind_fpath)
         self.meta_hybridizer = MetaHybridizer(
-            data=self.data, allow_solar_only=allow_solar_only,
-            allow_wind_only=allow_wind_only, fillna=fillna, limits=limits,
-            ratio_bounds=ratio_bounds, ratio=ratio
+            data=self.data,
+            allow_solar_only=allow_solar_only,
+            allow_wind_only=allow_wind_only,
+            fillna=fillna,
+            limits=limits,
+            ratio_bounds=ratio_bounds,
+            ratio=ratio,
         )
         self._profiles = None
         self._validate_input()
 
     def _validate_input(self):
-        """Validate the user input and input files. """
+        """Validate the user input and input files."""
         self.data.validate()
         self.meta_hybridizer.validate_input()
 
     @property
     def solar_meta(self):
         """Summary for the solar representative profiles.
 
@@ -1038,15 +1128,15 @@
 
         self.run_meta()
         self.run_profiles()
 
         if fout is not None:
             self.save_profiles(fout, save_hybrid_meta=save_hybrid_meta)
 
-        logger.info('Hybridization of representative profiles complete!')
+        logger.info("Hybridization of representative profiles complete!")
         return fout
 
     def run_meta(self):
         """Compute the hybridized profiles.
 
         Returns
         -------
@@ -1063,62 +1153,76 @@
         Returns
         -------
         `Hybridization`
             Instance of Hybridization object (itself) containing the
             hybridized profiles as attributes.
         """
 
-        logger.info('Running hybrid profile calculations.')
+        logger.info("Running hybrid profile calculations.")
 
         self._init_profiles()
         self._compute_hybridized_profile_components()
         self._compute_hybridized_profiles_from_components()
 
-        logger.info('Profile hybridization complete.')
+        logger.info("Profile hybridization complete.")
 
         return self
 
     def _init_profiles(self):
         """Initialize the output rep profiles attribute."""
         self._profiles = {
-            k: np.zeros((len(self.hybrid_time_index), len(self.hybrid_meta)),
-                        dtype=np.float32)
-            for k in OUTPUT_PROFILE_NAMES}
+            k: np.zeros(
+                (len(self.hybrid_time_index), len(self.hybrid_meta)),
+                dtype=np.float32,
+            )
+            for k in OUTPUT_PROFILE_NAMES
+        }
 
     def _compute_hybridized_profile_components(self):
-        """Compute the resource components of the hybridized profiles. """
+        """Compute the resource components of the hybridized profiles."""
 
         for params in self.__rep_profile_hybridization_params:
             col, (hybrid_idxs, solar_idxs), fpath, p_name, dset_name = params
             capacity = self.hybrid_meta.loc[hybrid_idxs, col].values
 
             with Resource(fpath) as res:
-                data = res[dset_name,
-                           res.time_index.isin(self.hybrid_time_index)]
-                self._profiles[p_name][:, hybrid_idxs] = (data[:, solar_idxs]
-                                                          * capacity)
+                data = res[
+                    dset_name, res.time_index.isin(self.hybrid_time_index)
+                ]
+                self._profiles[p_name][:, hybrid_idxs] = (
+                    data[:, solar_idxs] * capacity
+                )
 
     @property
     def __rep_profile_hybridization_params(self):
-        """Zip the rep profile hybridization parameters. """
+        """Zip the rep profile hybridization parameters."""
 
-        cap_col_names = ['hybrid_solar_capacity', 'hybrid_wind_capacity']
-        idx_maps = [self.meta_hybridizer.solar_profile_indices_map,
-                    self.meta_hybridizer.wind_profile_indices_map]
+        cap_col_names = [f"hybrid_solar_{SupplyCurveField.CAPACITY}",
+                         f"hybrid_wind_{SupplyCurveField.CAPACITY}"]
+        idx_maps = [
+            self.meta_hybridizer.solar_profile_indices_map,
+            self.meta_hybridizer.wind_profile_indices_map,
+        ]
         fpaths = [self.data.solar_fpath, self.data.wind_fpath]
-        zipped = zip(cap_col_names, idx_maps, fpaths, OUTPUT_PROFILE_NAMES[1:],
-                     self.data.profile_dset_names)
+        zipped = zip(
+            cap_col_names,
+            idx_maps,
+            fpaths,
+            OUTPUT_PROFILE_NAMES[1:],
+            self.data.profile_dset_names,
+        )
         return zipped
 
     def _compute_hybridized_profiles_from_components(self):
-        """Compute the hybridized profiles from the resource components. """
+        """Compute the hybridized profiles from the resource components."""
 
         hp_name, sp_name, wp_name = OUTPUT_PROFILE_NAMES
-        self._profiles[hp_name] = (self._profiles[sp_name]
-                                   + self._profiles[wp_name])
+        self._profiles[hp_name] = (
+            self._profiles[sp_name] + self._profiles[wp_name]
+        )
 
     def _init_h5_out(self, fout, save_hybrid_meta=True):
         """Initialize an output h5 file for hybrid profiles.
 
         Parameters
         ----------
         fout : str
@@ -1142,38 +1246,50 @@
         meta = self.hybrid_meta.copy()
         for c in meta.columns:
             try:
                 meta[c] = pd.to_numeric(meta[c])
             except ValueError:
                 pass
 
-        Outputs.init_h5(fout, dsets, shapes, attrs, chunks, dtypes,
-                        meta, time_index=self.hybrid_time_index)
+        Outputs.init_h5(
+            fout,
+            dsets,
+            shapes,
+            attrs,
+            chunks,
+            dtypes,
+            meta,
+            time_index=self.hybrid_time_index,
+        )
 
         if save_hybrid_meta:
-            with Outputs(fout, mode='a') as out:
+            with Outputs(fout, mode="a") as out:
                 hybrid_meta = to_records_array(self.hybrid_meta)
-                out._create_dset('meta', hybrid_meta.shape,
-                                 hybrid_meta.dtype, data=hybrid_meta)
+                out._create_dset(
+                    "meta",
+                    hybrid_meta.shape,
+                    hybrid_meta.dtype,
+                    data=hybrid_meta,
+                )
 
     def _write_h5_out(self, fout, save_hybrid_meta=True):
         """Write hybrid profiles and meta to an output file.
 
         Parameters
         ----------
         fout : str
             Filepath to output h5 file.
         save_hybrid_meta : bool
             Flag to save hybrid SC table to hybrid rep profile output.
         """
 
-        with Outputs(fout, mode='a') as out:
-            if 'meta' in out.datasets and save_hybrid_meta:
+        with Outputs(fout, mode="a") as out:
+            if "meta" in out.datasets and save_hybrid_meta:
                 hybrid_meta = to_records_array(self.hybrid_meta)
-                out['meta'] = hybrid_meta
+                out["meta"] = hybrid_meta
 
             for dset, data in self.profiles.items():
                 out[dset] = data
 
     def save_profiles(self, fout, save_hybrid_meta=True):
         """Initialize fout and save profiles.
```

### Comparing `NREL-reV-0.8.7/reV/losses/power_curve.py` & `NREL-reV-0.8.9/reV/losses/power_curve.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/losses/scheduled.py` & `NREL-reV-0.8.9/reV/losses/scheduled.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/losses/utils.py` & `NREL-reV-0.8.9/reV/losses/utils.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/nrwal/cli_nrwal.py` & `NREL-reV-0.8.9/reV/nrwal/cli_nrwal.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/nrwal/nrwal.py` & `NREL-reV-0.8.9/reV/nrwal/nrwal.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,41 @@
 first developed to use a custom offshore wind LCOE equation library but has
 since been refactored to analyze any equation library in NRWAL.
 
 Everything in this module operates on the spatiotemporal resolution of the reV
 generation output file. This is usually the wind or solar resource resolution
 but could be the supply curve resolution after representative profiles is run.
 """
-import numpy as np
-import pandas as pd
 import logging
 from warnings import warn
 
+import numpy as np
+import pandas as pd
+
 from reV.generation.generation import Gen
 from reV.handlers.outputs import Outputs
-from reV.utilities.exceptions import (DataShapeError,
-                                      OffshoreWindInputWarning,
-                                      OffshoreWindInputError)
-from reV.utilities import log_versions
-
+from reV.utilities import SiteDataField, ResourceMetaField, log_versions
+from reV.utilities.exceptions import (
+    DataShapeError,
+    OffshoreWindInputError,
+    OffshoreWindInputWarning,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class RevNrwal:
     """RevNrwal"""
 
-    DEFAULT_META_COLS = ('config', )
+    DEFAULT_META_COLS = (SiteDataField.CONFIG, )
     """Columns from the `site_data` table to join to the output meta data"""
 
     def __init__(self, gen_fpath, site_data, sam_files, nrwal_configs,
-                 output_request, save_raw=True, meta_gid_col='gid',
+                 output_request, save_raw=True,
+                 meta_gid_col=ResourceMetaField.GID,
                  site_meta_cols=None):
         """Framework to handle reV-NRWAL analysis.
 
         ``reV`` NRWAL analysis runs ``reV`` data through the NRWAL
         compute library. Everything in this module operates on the
         spatiotemporal resolution of the ``reV`` generation output file
         (usually the wind or solar resource resolution but could also be
@@ -159,43 +162,51 @@
         self._site_data = site_data
         self._output_request = output_request
         self._meta_out = None
         self._time_index = None
         self._save_raw = save_raw
         self._nrwal_inputs = self._out = None
 
-        self._nrwal_configs = {k: NrwalConfig(v) for k, v in
-                               nrwal_configs.items()}
+        self._nrwal_configs = {
+            k: NrwalConfig(v) for k, v in nrwal_configs.items()
+        }
 
         self._site_meta_cols = site_meta_cols
         if self._site_meta_cols is None:
             self._site_meta_cols = list(self.DEFAULT_META_COLS)
         else:
             self._site_meta_cols = list(self._site_meta_cols)
             self._site_meta_cols += list(self.DEFAULT_META_COLS)
             self._site_meta_cols = list(set(self._site_meta_cols))
 
         self._site_data = self._parse_site_data()
         self._meta_source = self._parse_gen_data()
         self._analysis_gids, self._site_data = self._parse_analysis_gids()
 
-        pc = Gen.get_pc(self._site_data[['gid', 'config']], points_range=None,
-                        sam_configs=sam_files, tech='windpower')
+        pc = Gen.get_pc(
+            self._site_data[[SiteDataField.GID, SiteDataField.CONFIG]],
+            points_range=None, sam_configs=sam_files, tech='windpower')
         self._project_points = pc.project_points
 
         self._sam_sys_inputs = self._parse_sam_sys_inputs()
         meta_gids = self.meta_source[self._meta_gid_col].values
-        logger.info('Finished initializing NRWAL analysis module for "{}" '
-                    '{} through {} with {} total generation points and '
-                    '{} NRWAL analysis points.'
-                    .format(self._meta_gid_col, meta_gids.min(),
-                            meta_gids.max(), len(self.meta_source),
-                            len(self.analysis_gids)))
+        logger.info(
+            'Finished initializing NRWAL analysis module for "{}" '
+            "{} through {} with {} total generation points and "
+            "{} NRWAL analysis points.".format(
+                self._meta_gid_col,
+                meta_gids.min(),
+                meta_gids.max(),
+                len(self.meta_source),
+                len(self.analysis_gids),
+            )
+        )
 
-    def _parse_site_data(self, required_columns=('gid', 'config')):
+    def _parse_site_data(self, required_columns=(SiteDataField.GID,
+                                                 SiteDataField.CONFIG)):
         """Parse the site-specific spatial input data file
 
         Parameters
         ----------
         required_columns : tuple | list
             List of column names that must be in the site_data in
             order to run the reV NRWAL module.
@@ -206,54 +217,60 @@
             Dataframe of extracted site_data. Each row is an analysis point and
             columns are spatial data inputs.
         """
 
         if isinstance(self._site_data, str):
             self._site_data = pd.read_csv(self._site_data)
 
-        if 'dist_l_to_ts' in self._site_data:
-            if self._site_data['dist_l_to_ts'].sum() > 0:
-                w = ('Possible incorrect Offshore data input! "dist_l_to_ts" '
-                     '(distance land to transmission) input is non-zero. '
-                     'Most reV runs set this to zero and input the cost '
-                     'of transmission from landfall tie-in to '
-                     'transmission feature in the supply curve module.')
+        if "dist_l_to_ts" in self._site_data:
+            if self._site_data["dist_l_to_ts"].sum() > 0:
+                w = (
+                    'Possible incorrect Offshore data input! "dist_l_to_ts" '
+                    "(distance land to transmission) input is non-zero. "
+                    "Most reV runs set this to zero and input the cost "
+                    "of transmission from landfall tie-in to "
+                    "transmission feature in the supply curve module."
+                )
                 logger.warning(w)
                 warn(w, OffshoreWindInputWarning)
 
         for c in required_columns:
             if c not in self._site_data:
-                msg = ('Did not find required "{}" column in site_data!'
-                       .format(c))
+                msg = 'Did not find required "{}" column in site_data!'.format(
+                    c
+                )
                 logger.error(msg)
                 raise KeyError(msg)
 
-        self._site_data = self._site_data.sort_values('gid')
+        self._site_data = self._site_data.sort_values(SiteDataField.GID)
 
         return self._site_data
 
     def _parse_gen_data(self):
         """Parse generation data and get meta data
 
         Returns
         -------
         meta : pd.DataFrame
             Full meta data from gen_fpath.
         """
 
-        with Outputs(self._gen_fpath, mode='r') as out:
+        with Outputs(self._gen_fpath, mode="r") as out:
             meta = out.meta
 
-        msg = ('Could not find "{}" column in source generation h5 file '
-               'meta data! Available cols: {}'
-               .format(self._meta_gid_col, meta.columns.values.tolist()))
+        msg = (
+            'Could not find "{}" column in source generation h5 file '
+            "meta data! Available cols: {}".format(
+                self._meta_gid_col, meta.columns.values.tolist()
+            )
+        )
         assert self._meta_gid_col in meta, msg
 
         # currently an assumption of sorted gids in the reV gen output
-        msg = ('Source capacity factor meta data is not ordered!')
+        msg = "Source capacity factor meta data is not ordered!"
         meta_gids = list(meta[self._meta_gid_col])
         assert meta_gids == sorted(meta_gids), msg
 
         return meta
 
     def _parse_analysis_gids(self):
         """Check the intersection of the generation gids and the site_data
@@ -268,35 +285,39 @@
         site_data : pd.DataFrame
             The site_data table reduced to only those gids that are in the
             analysis_gids
         """
 
         meta_gids = self.meta_source[self._meta_gid_col].values
 
-        missing = ~np.isin(meta_gids, self._site_data['gid'])
+        missing = ~np.isin(meta_gids, self._site_data[SiteDataField.GID])
         if any(missing):
-            msg = ('{} sites from the generation meta data input were '
-                   'missing from the "site_data" input and will not be '
-                   'run through NRWAL: {}'
-                   .format(missing.sum(), meta_gids[missing]))
+            msg = (
+                "{} sites from the generation meta data input were "
+                'missing from the "site_data" input and will not be '
+                "run through NRWAL: {}".format(
+                    missing.sum(), meta_gids[missing]
+                )
+            )
             logger.info(msg)
 
-        missing = ~np.isin(self._site_data['gid'], meta_gids)
+        missing = ~np.isin(self._site_data[SiteDataField.GID], meta_gids)
         if any(missing):
-            missing = self._site_data['gid'].values[missing]
+            missing = self._site_data[SiteDataField.GID].values[missing]
             msg = ('{} sites from the "site_data" input were missing from the '
                    'generation meta data and will not be run through NRWAL: {}'
                    .format(len(missing), missing))
             logger.info(msg)
 
-        analysis_gids = set(meta_gids) & set(self._site_data['gid'])
+        analysis_gids = (set(meta_gids)
+                         & set(self._site_data[SiteDataField.GID]))
         analysis_gids = np.array(sorted(list(analysis_gids)))
 
         # reduce the site data table to only those sites being analyzed
-        mask = np.isin(self._site_data['gid'], meta_gids)
+        mask = np.isin(self._site_data[SiteDataField.GID], meta_gids)
         self._site_data = self._site_data[mask]
 
         return analysis_gids, self._site_data
 
     def _parse_sam_sys_inputs(self):
         """Get the SAM system inputs dict from project points.
 
@@ -311,17 +332,17 @@
         system_inputs = {}
 
         for gid in self.analysis_gids:
             system_inputs[gid] = self._project_points[gid][1]
 
         system_inputs = pd.DataFrame(system_inputs).T
         system_inputs = system_inputs.sort_index()
-        system_inputs['gid'] = system_inputs.index.values
-        system_inputs.index.name = 'gid'
-        mask = system_inputs['gid'].isin(self.analysis_gids)
+        system_inputs[SiteDataField.GID] = system_inputs.index.values
+        system_inputs.index.name = SiteDataField.GID
+        mask = system_inputs[SiteDataField.GID].isin(self.analysis_gids)
         system_inputs = system_inputs[mask]
 
         return system_inputs
 
     def _init_outputs(self):
         """Initialize a dictionary of outputs with dataset names as keys and
         numpy arrays as values. All datasets are initialized as 1D arrays and
@@ -333,176 +354,211 @@
         -------
         out : dict
             Dictionary of output data
         """
         out = {}
 
         for key in self._output_request:
-            out[key] = np.full(len(self.analysis_gids), np.nan,
-                               dtype=np.float32)
+            out[key] = np.full(
+                len(self.analysis_gids), np.nan, dtype=np.float32
+            )
 
             if key in self.gen_dsets and not self._save_raw:
-                msg = ('Output request "{0}" was also found in '
-                       'the source gen file but save_raw=False! If '
-                       'you are manipulating this '
-                       'dset, make sure you set save_raw=False '
-                       'and reference "{0}_raw" as the '
-                       'input in the NRWAL equations and then define "{0}" '
-                       'as the final manipulated dataset.'.format(key))
+                msg = (
+                    'Output request "{0}" was also found in '
+                    "the source gen file but save_raw=False! If "
+                    "you are manipulating this "
+                    "dset, make sure you set save_raw=False "
+                    'and reference "{0}_raw" as the '
+                    'input in the NRWAL equations and then define "{0}" '
+                    "as the final manipulated dataset.".format(key)
+                )
                 logger.warning(msg)
                 warn(msg)
             elif key in self.gen_dsets:
-                msg = ('Output request "{0}" was also found in '
-                       'the source gen file. If you are manipulating this '
-                       'dset, make sure you reference "{0}_raw" as the '
-                       'input in the NRWAL equations and then define "{0}" '
-                       'as the final manipulated dataset.'.format(key))
+                msg = (
+                    'Output request "{0}" was also found in '
+                    "the source gen file. If you are manipulating this "
+                    'dset, make sure you reference "{0}_raw" as the '
+                    'input in the NRWAL equations and then define "{0}" '
+                    "as the final manipulated dataset.".format(key)
+                )
                 logger.info(msg)
 
             if key in self._nrwal_inputs:
                 out[key] = self._nrwal_inputs[key]
 
         return out
 
     def _preflight_checks(self):
         """Run some preflight checks on the offshore inputs"""
-        sam_files = {k: v for k, v in
-                     self._project_points.sam_inputs.items()
-                     if k in self._nrwal_configs}
+        sam_files = {
+            k: v
+            for k, v in self._project_points.sam_inputs.items()
+            if k in self._nrwal_configs
+        }
 
         for cid, sys_in in sam_files.items():
-            loss1 = sys_in.get('wind_farm_losses_percent', 0)
-            loss2 = sys_in.get('turb_generic_loss', 0)
+            loss1 = sys_in.get("wind_farm_losses_percent", 0)
+            loss2 = sys_in.get("turb_generic_loss", 0)
             if loss1 != 0 or loss2 != 0:
-                msg = ('Wind farm loss for config "{}" is not 0. When using '
-                       'NRWAL for offshore analysis, consider using gross '
-                       'capacity factors from reV generation and applying '
-                       'spatially dependent losses from the NRWAL equations'
-                       .format(cid))
+                msg = (
+                    'Wind farm loss for config "{}" is not 0. When using '
+                    "NRWAL for offshore analysis, consider using gross "
+                    "capacity factors from reV generation and applying "
+                    "spatially dependent losses from the NRWAL equations"
+                    .format(cid)
+                )
                 logger.info(msg)
 
         available_ids = list(self._nrwal_configs.keys())
-        requested_ids = list(self._site_data['config'].values)
+        requested_ids = list(self._site_data[SiteDataField.CONFIG].values)
         missing = set(requested_ids) - set(available_ids)
         if any(missing):
-            msg = ('The following config ids were requested in the offshore '
-                   'data input but were not available in the NRWAL config '
-                   'input dict: {}'.format(missing))
+            msg = (
+                "The following config ids were requested in the offshore "
+                "data input but were not available in the NRWAL config "
+                "input dict: {}".format(missing)
+            )
             logger.error(msg)
             raise OffshoreWindInputError(msg)
 
-        check_gid_order = (self._site_data['gid'].values
-                           == self._sam_sys_inputs['gid'].values)
+        check_gid_order = (self._site_data[SiteDataField.GID].values
+                           == self._sam_sys_inputs[SiteDataField.GID].values)
         msg = 'NRWAL site_data and system input dataframe had bad order'
         assert (check_gid_order).all(), msg
 
         missing = [c for c in self._site_meta_cols if c not in self._site_data]
         if any(missing):
-            msg = ('Could not find requested NRWAL site data pass through '
-                   'columns in offshore input data: {}'.format(missing))
+            msg = (
+                "Could not find requested NRWAL site data pass through "
+                "columns in offshore input data: {}".format(missing)
+            )
             logger.error(msg)
             raise OffshoreWindInputError(msg)
 
     def _get_input_data(self):
         """Get all the input data from the site_data, SAM system configs, and
         generation h5 file, formatted together in one dictionary for NRWAL.
 
         Returns
         -------
         nrwal_inputs : dict
             Dictionary mapping required NRWAL input variable names (keys) to 1
             or 2D arrays of inputs for all the analysis_gids
         """
 
-        logger.info('Setting up input data for NRWAL...')
+        logger.info("Setting up input data for NRWAL...")
 
         # preconditions for this to work properly
         assert len(self._site_data) == len(self.analysis_gids)
         assert len(self._sam_sys_inputs) == len(self.analysis_gids)
 
         all_required = []
         for config_id, nrwal_config in self._nrwal_configs.items():
             all_required += list(nrwal_config.required_inputs)
             all_required = list(set(all_required))
 
-            missing_vars = [var for var in nrwal_config.required_inputs
-                            if var not in self._site_data
-                            and var not in self.meta_source
-                            and var not in self._sam_sys_inputs
-                            and var not in self.gen_dsets]
+            missing_vars = [
+                var
+                for var in nrwal_config.required_inputs
+                if var not in self._site_data
+                and var not in self.meta_source
+                and var not in self._sam_sys_inputs
+                and var not in self.gen_dsets
+            ]
 
             if any(missing_vars):
-                msg = ('Could not find required input variables {} '
-                       'for NRWAL config "{}" in either the offshore '
-                       'data or the SAM system data!'
-                       .format(missing_vars, config_id))
+                msg = (
+                    "Could not find required input variables {} "
+                    'for NRWAL config "{}" in either the offshore '
+                    "data or the SAM system data!".format(
+                        missing_vars, config_id
+                    )
+                )
                 logger.error(msg)
                 raise OffshoreWindInputError(msg)
 
-        meta_data_vars = [var for var in all_required
-                          if var in self.meta_source]
-        logger.info('Pulling the following inputs from the gen meta data: {}'
-                    .format(meta_data_vars))
-        nrwal_inputs = {var: self.meta_source[var].values[self.analysis_mask]
-                        for var in meta_data_vars}
+        meta_data_vars = [
+            var for var in all_required if var in self.meta_source
+        ]
+        logger.info(
+            "Pulling the following inputs from the gen meta data: {}".format(
+                meta_data_vars
+            )
+        )
+        nrwal_inputs = {
+            var: self.meta_source[var].values[self.analysis_mask]
+            for var in meta_data_vars
+        }
 
         site_data_vars = [var for var in all_required
                           if var in self._site_data
                           and var not in nrwal_inputs]
-        site_data_vars.append('config')
+        site_data_vars.append(SiteDataField.CONFIG)
         logger.info('Pulling the following inputs from the site_data input: {}'
                     .format(site_data_vars))
         for var in site_data_vars:
             nrwal_inputs[var] = self._site_data[var].values
 
-        sam_sys_vars = [var for var in all_required
-                        if var in self._sam_sys_inputs
-                        and var not in nrwal_inputs]
-        logger.info('Pulling the following inputs from the SAM system '
-                    'configs: {}'.format(sam_sys_vars))
+        sam_sys_vars = [
+            var
+            for var in all_required
+            if var in self._sam_sys_inputs and var not in nrwal_inputs
+        ]
+        logger.info(
+            "Pulling the following inputs from the SAM system "
+            "configs: {}".format(sam_sys_vars)
+        )
         for var in sam_sys_vars:
             nrwal_inputs[var] = self._sam_sys_inputs[var].values
 
-        gen_vars = [var for var in all_required
-                    if var in self.gen_dsets
-                    and var not in nrwal_inputs]
-        logger.info('Pulling the following inputs from the generation '
-                    'h5 file: {}'.format(gen_vars))
-        with Outputs(self._gen_fpath, mode='r') as f:
+        gen_vars = [
+            var
+            for var in all_required
+            if var in self.gen_dsets and var not in nrwal_inputs
+        ]
+        logger.info(
+            "Pulling the following inputs from the generation "
+            "h5 file: {}".format(gen_vars)
+        )
+        with Outputs(self._gen_fpath, mode="r") as f:
             source_gids = self.meta_source[self._meta_gid_col]
             gen_gids = np.where(source_gids.isin(self.analysis_gids))[0]
             for var in gen_vars:
                 shape = f.shapes[var]
                 if len(shape) == 1:
                     nrwal_inputs[var] = f[var, gen_gids]
                 elif len(shape) == 2:
                     nrwal_inputs[var] = f[var, :, gen_gids]
                 else:
-                    msg = ('Data shape for "{}" must be 1 or 2D but '
-                           'received: {}'.format(var, shape))
+                    msg = (
+                        'Data shape for "{}" must be 1 or 2D but '
+                        "received: {}".format(var, shape)
+                    )
                     logger.error(msg)
                     raise DataShapeError(msg)
 
-        logger.info('Finished setting up input data for NRWAL!')
+        logger.info("Finished setting up input data for NRWAL!")
 
         return nrwal_inputs
 
     @property
     def time_index(self):
         """Get the source time index."""
         if self._time_index is None:
-            with Outputs(self._gen_fpath, mode='r') as out:
+            with Outputs(self._gen_fpath, mode="r") as out:
                 self._time_index = out.time_index
 
         return self._time_index
 
     @property
     def gen_dsets(self):
         """Get the available datasets from the gen source file"""
-        with Outputs(self._gen_fpath, mode='r') as out:
+        with Outputs(self._gen_fpath, mode="r") as out:
             dsets = out.dsets
 
         return dsets
 
     @property
     def meta_source(self):
         """Get the full meta data (onshore + offshore)"""
@@ -524,16 +580,17 @@
         """Get a boolean array to mask the source generation meta data where
         True is sites that are to be analyzed by NRWAL.
 
         Returns
         -------
         np.ndarray
         """
-        mask = np.isin(self.meta_source[self._meta_gid_col],
-                       self.analysis_gids)
+        mask = np.isin(
+            self.meta_source[self._meta_gid_col], self.analysis_gids
+        )
         return mask
 
     @property
     def analysis_gids(self):
         """Get an array of gids from the source generation meta data that are
         to-be analyzed by nrwal.
 
@@ -572,30 +629,35 @@
 
         if len(value.shape) == 1:
             self._out[name][output_mask] = value[output_mask]
 
         elif len(value.shape) == 2:
             if len(self._out[name].shape) == 1:
                 if not all(np.isnan(self._out[name])):
-                    msg = ('Output dataset "{}" was initialized as 1D but was '
-                           'later found to be 2D but was not all NaN!'
-                           .format(name))
+                    msg = (
+                        'Output dataset "{}" was initialized as 1D but was '
+                        "later found to be 2D but was not all NaN!".format(
+                            name
+                        )
+                    )
                     logger.error(msg)
                     raise DataShapeError(msg)
 
                 # re-initialize the dataset as 2D now that we
                 # know what the output looks like
                 out_shape = (len(self.time_index), len(self.analysis_gids))
                 self._out[name] = np.full(out_shape, np.nan, dtype=np.float32)
 
             self._out[name][:, output_mask] = value[:, output_mask]
 
         else:
-            msg = ('Could not make sense of NRWAL output "{}" '
-                   'with shape {}'.format(name, value.shape))
+            msg = (
+                'Could not make sense of NRWAL output "{}" '
+                "with shape {}".format(name, value.shape)
+            )
             logger.error(msg)
             raise DataShapeError(msg)
 
     def _save_nrwal_misc(self, name, nrwal_config, output_mask):
         """Save miscellaneous output requests from a NRWAL config object (not
         NRWAL output dictionary) to the self._out attribute.
 
@@ -610,47 +672,52 @@
             Boolean array showing which gids in self.analysis_gids should be
             assigned data from this NRWAL output. If not all true, there are
             probably multiple NrwalConfig objects that map to different sets of
             gids.
         """
 
         from NRWAL import Equation
+
         value = nrwal_config[name]
 
         if isinstance(value, Equation):
-            msg = ('Cannot retrieve Equation "{}" from NRWAL. '
-                   'Must be a number!'.format(name))
+            msg = (
+                'Cannot retrieve Equation "{}" from NRWAL. '
+                "Must be a number!".format(name)
+            )
             assert not any(value.variables), msg
             value = value.eval()
 
         value = self._value_to_array(value, name)
         self._out[name][output_mask] = value[output_mask]
 
     def _value_to_array(self, value, name):
         """Turn the input into numpy array if it isn't already."""
         if np.issubdtype(type(value), np.number):
             value *= np.ones(len(self.analysis_gids), dtype=np.float32)
 
         if not isinstance(value, np.ndarray):
-            msg = ('NRWAL key "{}" returned bad type of "{}", needs to be '
-                   'numeric or an output array.'.format(name, type(value)))
+            msg = (
+                'NRWAL key "{}" returned bad type of "{}", needs to be '
+                "numeric or an output array.".format(name, type(value))
+            )
             logger.error(msg)
             raise TypeError(msg)
         return value
 
     def run_nrwal(self):
         """Run analysis via the NRWAL analysis library"""
 
         self._preflight_checks()
         self.save_raw_dsets()
         self._nrwal_inputs = self._get_input_data()
         self._out = self._init_outputs()
 
         for i, (cid, nrwal_config) in enumerate(self._nrwal_configs.items()):
-            output_mask = self._site_data['config'].values == cid
+            output_mask = self._site_data[SiteDataField.CONFIG].values == cid
             logger.info('Running NRWAL config {} of {}: "{}" and applying '
                         'to {} out of {} total sites'
                         .format(i + 1, len(self._nrwal_configs), cid,
                                 output_mask.sum(), len(output_mask)))
 
             nrwal_out = nrwal_config.eval(inputs=self._nrwal_inputs)
 
@@ -659,103 +726,125 @@
                 if name in nrwal_out:
                     self._save_nrwal_out(name, nrwal_out, output_mask)
 
                 elif name in nrwal_config.keys():
                     self._save_nrwal_misc(name, nrwal_config, output_mask)
 
                 elif name not in self._nrwal_inputs:
-                    msg = ('Could not find "{}" in the output dict of NRWAL '
-                           'config {}'.format(name, cid))
+                    msg = (
+                        'Could not find "{}" in the output dict of NRWAL '
+                        "config {}".format(name, cid)
+                    )
                     logger.warning(msg)
                     warn(msg)
 
     def check_outputs(self):
         """Check the nrwal outputs for nan values and raise errors if found."""
         for name, arr in self._out.items():
             if np.isnan(arr).all():
-                msg = ('Output array "{}" is all NaN! Probably was not '
-                       'found in the available NRWAL keys.'.format(name))
+                msg = (
+                    'Output array "{}" is all NaN! Probably was not '
+                    "found in the available NRWAL keys.".format(name)
+                )
                 logger.warning(msg)
                 warn(msg)
             elif np.isnan(arr).any():
                 mask = np.isnan(arr)
                 nan_meta = self.meta_source[self.analysis_mask][mask]
                 nan_gids = nan_meta[self._meta_gid_col].values
-                msg = ('NaN values ({} out of {}) persist in NRWAL '
-                       'output "{}"!'
-                       .format(np.isnan(arr).sum(), len(arr), name))
+                msg = (
+                    "NaN values ({} out of {}) persist in NRWAL "
+                    'output "{}"!'.format(np.isnan(arr).sum(), len(arr), name)
+                )
                 logger.warning(msg)
-                logger.warning('This is the NRWAL meta that is causing NaN '
-                               'outputs: {}'.format(nan_meta))
-                logger.warning('These are the resource gids causing NaN '
-                               'outputs: {}'.format(nan_gids))
+                logger.warning(
+                    "This is the NRWAL meta that is causing NaN "
+                    "outputs: {}".format(nan_meta)
+                )
+                logger.warning(
+                    "These are the resource gids causing NaN "
+                    "outputs: {}".format(nan_gids)
+                )
                 warn(msg)
 
     def save_raw_dsets(self):
         """If requested by save_raw=True, archive raw datasets that exist in
         the gen_fpath file and are also requested in the output_request"""
         if self._save_raw:
-            with Outputs(self._gen_fpath, 'a') as f:
+            with Outputs(self._gen_fpath, "a") as f:
                 for dset in self._output_request:
-                    dset_raw = '{}_raw'.format(dset)
+                    dset_raw = "{}_raw".format(dset)
                     if dset in f and dset_raw not in f:
-                        logger.info('Saving raw data from "{}" to "{}"'
-                                    .format(dset, dset_raw))
-                        f._add_dset(dset_raw, f[dset], f.dtypes[dset],
-                                    attrs=f.attrs[dset])
+                        logger.info(
+                            'Saving raw data from "{}" to "{}"'.format(
+                                dset, dset_raw
+                            )
+                        )
+                        f._add_dset(
+                            dset_raw,
+                            f[dset],
+                            f.dtypes[dset],
+                            attrs=f.attrs[dset],
+                        )
 
     def write_to_gen_fpath(self):
         """Save NRWAL outputs to input generation fpath file.
 
         Returns
         -------
         str
             Path to output file.
         """
 
-        logger.info('Writing NRWAL outputs to: {}'.format(self._gen_fpath))
+        logger.info("Writing NRWAL outputs to: {}".format(self._gen_fpath))
         write_all = self.analysis_mask.all()
 
-        with Outputs(self._gen_fpath, 'a') as f:
-            meta_attrs = f.attrs['meta']
-            del f._h5['meta']
-            f._set_meta('meta', self.meta_out, attrs=meta_attrs)
+        with Outputs(self._gen_fpath, "a") as f:
+            meta_attrs = f.attrs["meta"]
+            del f._h5["meta"]
+            f._set_meta("meta", self.meta_out, attrs=meta_attrs)
 
             for dset, arr in self._out.items():
                 if len(arr.shape) == 1:
-                    data = np.full(len(self.meta_source), np.nan,
-                                   dtype=np.float32)
+                    data = np.full(
+                        len(self.meta_source), np.nan, dtype=np.float32
+                    )
                 else:
-                    full_shape = (len(self.time_index),
-                                  len(self.meta_source))
+                    full_shape = (len(self.time_index), len(self.meta_source))
                     data = np.full(full_shape, np.nan, dtype=np.float32)
 
-                dset_attrs = {'scale_factor': 1}
+                dset_attrs = {"scale_factor": 1}
                 dset_dtype = np.float32
                 if dset in f.dsets:
-                    logger.info('Found "{}" in file, loading data and '
-                                'overwriting data for {} out of {} sites.'
-                                .format(dset, self.analysis_mask.sum(),
-                                        len(self.analysis_mask)))
+                    logger.info(
+                        'Found "{}" in file, loading data and '
+                        "overwriting data for {} out of {} sites.".format(
+                            dset,
+                            self.analysis_mask.sum(),
+                            len(self.analysis_mask),
+                        )
+                    )
                     dset_attrs = f.attrs[dset]
                     dset_dtype = f.dtypes[dset]
                     if not write_all:
                         data = f[dset]
 
                 if len(arr.shape) == 1:
                     data[self.analysis_mask] = arr
                 else:
                     data[:, self.analysis_mask] = arr
 
-                logger.info('Writing final "{}" to: {}'
-                            .format(dset, self._gen_fpath))
+                logger.info(
+                    'Writing final "{}" to: {}'.format(dset, self._gen_fpath)
+                )
                 f._add_dset(dset, data, dset_dtype, attrs=dset_attrs)
 
-        logger.info('Finished writing NRWAL outputs to: {}'
-                    .format(self._gen_fpath))
+        logger.info(
+            "Finished writing NRWAL outputs to: {}".format(self._gen_fpath)
+        )
         return self._gen_fpath
 
     def write_meta_to_csv(self, out_fpath=None):
         """Combine NRWAL outputs with meta and write to output csv.
 
         Parameters
         ----------
@@ -772,29 +861,32 @@
             Path to output file.
         """
         if out_fpath is None:
             out_fpath = self._gen_fpath.replace(".h5", ".csv")
         elif not out_fpath.endswith(".csv"):
             out_fpath = "{}.csv".format(out_fpath)
 
-        logger.info('Writing NRWAL outputs to: {}'.format(out_fpath))
+        logger.info("Writing NRWAL outputs to: {}".format(out_fpath))
         meta_out = self.meta_out[self.analysis_mask].copy()
 
         for dset, arr in self._out.items():
             if len(arr.shape) != 1 or arr.shape[0] != meta_out.shape[0]:
-                msg = ('Skipping output {!r}: shape {} cannot be combined '
-                       'with meta of shape {}!'
-                       .format(dset, arr.shape, meta_out.shape))
+                msg = (
+                    "Skipping output {!r}: shape {} cannot be combined "
+                    "with meta of shape {}!".format(
+                        dset, arr.shape, meta_out.shape
+                    )
+                )
                 logger.warning(msg)
                 warn(msg)
                 continue
             meta_out[dset] = arr
 
         meta_out.to_csv(out_fpath, index=False)
-        logger.info('Finished writing NRWAL outputs to: {}'.format(out_fpath))
+        logger.info("Finished writing NRWAL outputs to: {}".format(out_fpath))
         return out_fpath
 
     def run(self, csv_output=False, out_fpath=None):
         """Run NRWAL analysis.
 
         Parameters
         ----------
@@ -827,24 +919,26 @@
 
         Returns
         -------
         str
             Path to output file.
         """
         if csv_output and self._save_raw:
-            msg = ("`save_raw` option not allowed with `csv_output`. Setting"
-                   "`save_raw=False`")
+            msg = (
+                "`save_raw` option not allowed with `csv_output`. Setting"
+                "`save_raw=False`"
+            )
             logger.warning(msg)
             warn(msg)
             self._save_raw = False
 
         if any(self.analysis_gids):
             self.run_nrwal()
             self.check_outputs()
             if csv_output:
                 out_fp = self.write_meta_to_csv(out_fpath)
             else:
                 out_fp = self.write_to_gen_fpath()
 
-        logger.info('NRWAL module complete!')
+        logger.info("NRWAL module complete!")
 
         return out_fp
```

### Comparing `NREL-reV-0.8.7/reV/qa_qc/cli_qa_qc.py` & `NREL-reV-0.8.9/reV/qa_qc/cli_qa_qc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # -*- coding: utf-8 -*-
 """
 QA/QC CLI utility functions.
 """
-import click
 import logging
-import numpy as np
 import os
 
-from rex.utilities.cli_dtypes import STR, STRLIST, INT
+import click
+import numpy as np
+from gaps.cli import CLICommandFromFunction, as_click_command
+from rex.utilities.cli_dtypes import INT, STR, STRLIST
 from rex.utilities.loggers import init_logger
-from gaps.cli import as_click_command, CLICommandFromFunction
 
-from reV.utilities import ModuleName
-from reV.qa_qc.qa_qc import QaQc, QaQcModule
-from reV.qa_qc.summary import (SummarizeH5, SummarizeSupplyCurve,
-                               SupplyCurvePlot, ExclusionsMask)
 from reV import __version__
+from reV.qa_qc.qa_qc import QaQc, QaQcModule
+from reV.qa_qc.summary import (
+    ExclusionsMask,
+    SummarizeH5,
+    SummarizeSupplyCurve,
+    SupplyCurvePlot,
+)
+from reV.utilities import ModuleName, SupplyCurveField
 
 logger = logging.getLogger(__name__)
 
 
 def cli_qa_qc(modules, out_dir, max_workers=None):
     """Run QA/QC on reV outputs
 
@@ -186,16 +190,16 @@
               help=("Path to .csv containing Supply Curve table, can be "
                     "supplied in 'supply-curve-table'"))
 @click.option('--plot_type', '-plt', default='plotly',
               type=click.Choice(['plot', 'plotly'], case_sensitive=False),
               show_default=True,
               help=(" plot_type of plot to create 'plot' or 'plotly', by "
                     "default 'plot'"))
-@click.option('--lcoe', '-lcoe', type=STR, default='mean_lcoe',
-              help="LCOE value to plot, by default 'mean_lcoe'")
+@click.option('--lcoe', '-lcoe', type=STR, default=SupplyCurveField.MEAN_LCOE,
+              help="LCOE value to plot, by default %(default)s")
 @click.pass_context
 def supply_curve_plot(ctx, sc_table, plot_type, lcoe):
     """
     Plot Supply Curve (cumulative capacity vs LCOE)
     """
     if sc_table is None:
         sc_table = ctx.obj['SC_TABLE']
```

### Comparing `NREL-reV-0.8.7/reV/qa_qc/summary.py` & `NREL-reV-0.8.9/reV/qa_qc/summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # -*- coding: utf-8 -*-
 """
 Compute and plot summary data
 """
 import logging
-import numpy as np
 import os
+
+import numpy as np
 import pandas as pd
-import plotting as mplt
 import plotly.express as px
-
+import plotting as mplt
 from rex import Resource
 from rex.utilities import SpawnProcessPool, parse_table
 
+from reV.utilities import SupplyCurveField, ResourceMetaField
+
 logger = logging.getLogger(__name__)
 
 
 class SummarizeH5:
     """
     reV Summary data for QA/QC
     """
+
     def __init__(self, h5_file, group=None):
         """
         Parameters
         ----------
         h5_file : str
             Path to .h5 file to summarize data from
         group : str, optional
             Group within h5_file to summarize datasets for, by default None
         """
-        logger.info('QAQC Summarize initializing on: {}'.format(h5_file))
+        logger.info("QAQC Summarize initializing on: {}".format(h5_file))
         self._h5_file = h5_file
         self._group = group
 
     def __repr__(self):
         msg = "{} for {}".format(self.__class__.__name__, self.h5_file)
 
         return msg
@@ -69,20 +72,20 @@
         sites_summary : pandas.DataFrame
             Summary stats for given sites / dataset
         """
         if sites is None:
             sites = slice(None)
 
         with Resource(h5_file, group=group) as f:
-            sites_meta = f['meta', sites]
+            sites_meta = f["meta", sites]
             sites_data = f[ds_name, :, sites]
 
         sites_summary = pd.DataFrame(sites_data, columns=sites_meta.index)
-        sites_summary = sites_summary.describe().T.drop(columns=['count'])
-        sites_summary['sum'] = sites_data.sum(axis=0)
+        sites_summary = sites_summary.describe().T.drop(columns=["count"])
+        sites_summary["sum"] = sites_data.sum(axis=0)
 
         return sites_summary
 
     @staticmethod
     def _compute_ds_summary(h5_file, ds_name, group=None):
         """
         Compute summary statistics for given dataset (assumed to be a vector)
@@ -101,21 +104,22 @@
         ds_summary : pandas.DataFrame
             Summary statistics for dataset
         """
         with Resource(h5_file, group=group) as f:
             ds_data = f[ds_name, :]
 
         ds_summary = pd.DataFrame(ds_data, columns=[ds_name])
-        ds_summary = ds_summary.describe().drop(['count'])
-        ds_summary.at['sum', ds_name] = ds_data.sum()
+        ds_summary = ds_summary.describe().drop(["count"])
+        ds_summary.at["sum", ds_name] = ds_data.sum()
 
         return ds_summary
 
-    def summarize_dset(self, ds_name, process_size=None, max_workers=None,
-                       out_path=None):
+    def summarize_dset(
+        self, ds_name, process_size=None, max_workers=None, out_path=None
+    ):
         """
         Compute dataset summary. If dataset is 2D compute temporal statistics
         for each site
 
         Parameters
         ----------
         ds_name : str
@@ -140,54 +144,60 @@
             sites = np.arange(ds_shape[1])
             if max_workers != 1:
                 if process_size is None and ds_chunks is not None:
                     process_size = ds_chunks[1]
                 if process_size is None:
                     process_size = ds_shape[-1]
 
-                sites = \
-                    np.array_split(sites,
-                                   int(np.ceil(len(sites) / process_size)))
-                loggers = [__name__, 'reV']
-                with SpawnProcessPool(max_workers=max_workers,
-                                      loggers=loggers) as ex:
+                sites = np.array_split(
+                    sites, int(np.ceil(len(sites) / process_size))
+                )
+                loggers = [__name__, "reV"]
+                with SpawnProcessPool(
+                    max_workers=max_workers, loggers=loggers
+                ) as ex:
                     futures = []
                     for site_slice in sites:
-                        futures.append(ex.submit(
-                            self._compute_sites_summary,
-                            self.h5_file, ds_name, sites=site_slice,
-                            group=self._group))
+                        futures.append(
+                            ex.submit(
+                                self._compute_sites_summary,
+                                self.h5_file,
+                                ds_name,
+                                sites=site_slice,
+                                group=self._group,
+                            )
+                        )
 
                     summary = [future.result() for future in futures]
 
                 summary = pd.concat(summary)
+            elif process_size is None:
+                summary = self._compute_sites_summary(self.h5_file,
+                                                      ds_name,
+                                                      sites=sites,
+                                                      group=self._group)
             else:
-                if process_size is None:
-                    summary = self._compute_sites_summary(self.h5_file,
-                                                          ds_name,
-                                                          sites=sites,
-                                                          group=self._group)
-                else:
-                    sites = np.array_split(
-                        sites, int(np.ceil(len(sites) / process_size)))
+                sites = np.array_split(
+                    sites, int(np.ceil(len(sites) / process_size)))
 
-                    summary = []
-                    for site_slice in sites:
-                        summary.append(self._compute_sites_summary(
-                            self.h5_file, ds_name,
-                            sites=site_slice,
-                            group=self._group))
+                summary = []
+                for site_slice in sites:
+                    summary.append(self._compute_sites_summary(
+                        self.h5_file, ds_name,
+                        sites=site_slice,
+                        group=self._group))
 
-                    summary = pd.concat(summary)
+                summary = pd.concat(summary)
 
-            summary.index.name = 'gid'
+            summary.index.name = ResourceMetaField.GID
 
         else:
-            summary = self._compute_ds_summary(self.h5_file, ds_name,
-                                               group=self._group)
+            summary = self._compute_ds_summary(
+                self.h5_file, ds_name, group=self._group
+            )
 
         if out_path is not None:
             summary.to_csv(out_path)
 
         return summary
 
     def summarize_means(self, out_path=None):
@@ -202,33 +212,40 @@
         Returns
         -------
         meta : pandas.DataFrame
             Meta data with means datasets added
         """
         with Resource(self.h5_file, group=self._group) as f:
             meta = f.meta
-            if 'gid' not in meta:
-                if meta.index.name != 'gid':
-                    meta.index.name = 'gid'
+            if ResourceMetaField.GID not in meta:
+                if meta.index.name != ResourceMetaField.GID:
+                    meta.index.name = ResourceMetaField.GID
 
                 meta = meta.reset_index()
 
             for ds_name in f.datasets:
                 shape, dtype, _ = f.get_dset_properties(ds_name)
                 if len(shape) == 1 and np.issubdtype(dtype, np.number):
                     meta[ds_name] = f[ds_name]
 
         if out_path is not None:
             meta.to_csv(out_path, index=False)
 
         return meta
 
     @classmethod
-    def run(cls, h5_file, out_dir, group=None, dsets=None,
-            process_size=None, max_workers=None):
+    def run(
+        cls,
+        h5_file,
+        out_dir,
+        group=None,
+        dsets=None,
+        process_size=None,
+        max_workers=None,
+    ):
         """
         Summarize all datasets in h5_file and dump to out_dir
 
         Parameters
         ----------
         h5_file : str
             Path to .h5 file to summarize data from
@@ -245,35 +262,42 @@
             by default None
         """
         if not os.path.exists(out_dir):
             os.makedirs(out_dir, exist_ok=True)
 
         if dsets is None:
             with Resource(h5_file, group=group) as f:
-                dsets = [dset for dset in f.datasets
-                         if dset not in ['meta', 'time_index']]
+                dsets = [
+                    dset
+                    for dset in f.datasets
+                    if dset not in ["meta", "time_index"]
+                ]
         elif isinstance(dsets, str):
             dsets = [dsets]
 
         summary = cls(h5_file)
         for ds_name in dsets:
-            out_path = os.path.join(out_dir,
-                                    "{}_summary.csv".format(ds_name))
-            summary.summarize_dset(ds_name, process_size=process_size,
-                                   max_workers=max_workers, out_path=out_path)
+            out_path = os.path.join(out_dir, "{}_summary.csv".format(ds_name))
+            summary.summarize_dset(
+                ds_name,
+                process_size=process_size,
+                max_workers=max_workers,
+                out_path=out_path,
+            )
 
-        out_path = os.path.basename(h5_file).replace('.h5', '_summary.csv')
+        out_path = os.path.basename(h5_file).replace(".h5", "_summary.csv")
         out_path = os.path.join(out_dir, out_path)
         summary.summarize_means(out_path=out_path)
 
 
 class SummarizeSupplyCurve:
     """
     Summarize Supply Curve table
     """
+
     def __init__(self, sc_table):
         self._sc_table = self._parse_summary(sc_table)
 
     def __repr__(self):
         msg = "{}".format(self.__class__.__name__)
 
         return msg
@@ -339,35 +363,35 @@
 
             sc_table = sc_table[columns]
 
         sc_table = sc_table.select_dtypes(include=np.number)
 
         sc_summary = []
         sc_stat = sc_table.mean(axis=0)
-        sc_stat.name = 'mean'
+        sc_stat.name = "mean"
         sc_summary.append(sc_stat)
 
         sc_stat = sc_table.std(axis=0)
-        sc_stat.name = 'stdev'
+        sc_stat.name = "stdev"
         sc_summary.append(sc_stat)
 
         sc_stat = sc_table.median(axis=0)
-        sc_stat.name = 'median'
+        sc_stat.name = "median"
         sc_summary.append(sc_stat)
 
         sc_stat = sc_table.min(axis=0)
-        sc_stat.name = 'min'
+        sc_stat.name = "min"
         sc_summary.append(sc_stat)
 
         sc_stat = sc_table.max(axis=0)
-        sc_stat.name = 'max'
+        sc_stat.name = "max"
         sc_summary.append(sc_stat)
 
         sc_stat = sc_table.sum(axis=0)
-        sc_stat.name = 'sum'
+        sc_stat.name = "sum"
         sc_summary.append(sc_stat)
 
         sc_summary = pd.concat(sc_summary, axis=1).T
 
         if out_path is not None:
             sc_summary.to_csv(out_path)
 
@@ -388,23 +412,24 @@
             Column(s) to summarize, if None summarize all numeric columns,
             by default None
         """
         if not os.path.exists(out_dir):
             os.makedirs(out_dir, exist_ok=True)
 
         summary = cls(sc_table)
-        out_path = os.path.basename(sc_table).replace('.csv', '_summary.csv')
+        out_path = os.path.basename(sc_table).replace(".csv", "_summary.csv")
         out_path = os.path.join(out_dir, out_path)
         summary.supply_curve_summary(columns=columns, out_path=out_path)
 
 
 class PlotBase:
     """
     QA/QC Plotting base class
     """
+
     def __init__(self, data):
         """
         Parameters
         ----------
         data : str | pandas.DataFrame | ndarray
             data to plot or file containing data to plot
         """
@@ -434,15 +459,15 @@
         Parameters
         ----------
         fig : plotly.Figure
             Plotly Figure object
         out_path : str
             File path to save plot to, can be a .html or static image
         """
-        if out_path.endswith('.html'):
+        if out_path.endswith(".html"):
             fig.write_html(out_path)
         else:
             fig.write_image(out_path)
 
     @staticmethod
     def _check_value(df, values, scatter=True):
         """
@@ -457,28 +482,30 @@
         scatter : bool, optional
             Flag to check for latitude and longitude columns, by default True
         """
         if isinstance(values, str):
             values = [values]
 
         if scatter:
-            values += ['latitude', 'longitude']
+            values += [SupplyCurveField.LATITUDE, SupplyCurveField.LONGITUDE]
 
         for value in values:
             if value not in df:
-                msg = ("{} is not a valid column in summary table:\n{}"
-                       .format(value, df))
+                msg = "{} is not a valid column in summary table:\n{}".format(
+                    value, df
+                )
                 logger.error(msg)
                 raise ValueError(msg)
 
 
 class SummaryPlots(PlotBase):
     """
     Plot summary data for QA/QC
     """
+
     def __init__(self, summary):
         """
         Parameters
         ----------
         summary : str | pandas.DataFrame
             Summary DataFrame or path to summary .csv
         """
@@ -502,15 +529,15 @@
 
         Returns
         -------
         list
         """
         return list(self.summary.columns)
 
-    def scatter_plot(self, value, cmap='viridis', out_path=None, **kwargs):
+    def scatter_plot(self, value, cmap="viridis", out_path=None, **kwargs):
         """
         Plot scatter plot of value versus longitude and latitude using
         pandas.plot.scatter
 
         Parameters
         ----------
         value : str
@@ -519,18 +546,19 @@
             Matplotlib colormap name, by default 'viridis'
         out_path : str, optional
             File path to save plot to, by default None
         kwargs : dict
             Additional kwargs for plotting.dataframes.df_scatter
         """
         self._check_value(self.summary, value)
-        mplt.df_scatter(self.summary, x='longitude', y='latitude', c=value,
-                        colormap=cmap, filename=out_path, **kwargs)
+        mplt.df_scatter(self.summary, x=SupplyCurveField.LONGITUDE,
+                        y=SupplyCurveField.LATITUDE, c=value, colormap=cmap,
+                        filename=out_path, **kwargs)
 
-    def scatter_plotly(self, value, cmap='Viridis', out_path=None, **kwargs):
+    def scatter_plotly(self, value, cmap="Viridis", out_path=None, **kwargs):
         """
         Plot scatter plot of value versus longitude and latitude using
         plotly
 
         Parameters
         ----------
         value : str
@@ -540,41 +568,45 @@
         out_path : str, optional
             File path to save plot to, can be a .html or static image,
             by default None
         kwargs : dict
             Additional kwargs for plotly.express.scatter
         """
         self._check_value(self.summary, value)
-        fig = px.scatter(self.summary, x='longitude', y='latitude',
-                         color=value, color_continuous_scale=cmap, **kwargs)
+        fig = px.scatter(self.summary, x=SupplyCurveField.LONGITUDE,
+                         y=SupplyCurveField.LATITUDE, color=value,
+                         color_continuous_scale=cmap, **kwargs)
         fig.update_layout(font=dict(family="Arial", size=18, color="black"))
 
         if out_path is not None:
             self._save_plotly(fig, out_path)
 
         fig.show()
 
-    def _extract_sc_data(self, lcoe='mean_lcoe'):
+    def _extract_sc_data(self, lcoe=SupplyCurveField.MEAN_LCOE):
         """
         Extract supply curve data
 
         Parameters
         ----------
         lcoe : str, optional
-            LCOE value to use for supply curve, by default 'mean_lcoe'
+            LCOE value to use for supply curve,
+            by default :obj:`SupplyCurveField.MEAN_LCOE`
 
         Returns
         -------
         sc_df : pandas.DataFrame
             Supply curve data
         """
-        values = ['capacity', lcoe]
+        values = [SupplyCurveField.CAPACITY, lcoe]
         self._check_value(self.summary, values, scatter=False)
         sc_df = self.summary[values].sort_values(lcoe)
-        sc_df['cumulative_capacity'] = sc_df['capacity'].cumsum()
+        sc_df['cumulative_capacity'] = (
+            sc_df[SupplyCurveField.CAPACITY].cumsum()
+        )
 
         return sc_df
 
     def dist_plot(self, value, out_path=None, **kwargs):
         """
         Plot distribution plot of value using seaborn.distplot
 
@@ -610,16 +642,23 @@
 
         if out_path is not None:
             self._save_plotly(fig, out_path, **kwargs)
 
         fig.show()
 
     @classmethod
-    def scatter(cls, summary_csv, out_dir, value, plot_type='plotly',
-                cmap='viridis', **kwargs):
+    def scatter(
+        cls,
+        summary_csv,
+        out_dir,
+        value,
+        plot_type="plotly",
+        cmap="viridis",
+        **kwargs,
+    ):
         """
         Create scatter plot for given value in summary table and save to
         out_dir
 
         Parameters
         ----------
         summary_csv : str
@@ -632,33 +671,39 @@
             plot_type of plot to create 'plot' or 'plotly', by default 'plotly'
         cmap : str, optional
             Colormap name, by default 'viridis'
         kwargs : dict
             Additional plotting kwargs
         """
         splt = cls(summary_csv)
-        if plot_type == 'plot':
-            out_path = os.path.basename(summary_csv).replace('.csv', '.png')
+        if plot_type == "plot":
+            out_path = os.path.basename(summary_csv).replace(".csv", ".png")
             out_path = os.path.join(out_dir, out_path)
-            splt.scatter_plot(value, cmap=cmap.lower(), out_path=out_path,
-                              **kwargs)
-        elif plot_type == 'plotly':
-            out_path = os.path.basename(summary_csv).replace('.csv', '.html')
+            splt.scatter_plot(
+                value, cmap=cmap.lower(), out_path=out_path, **kwargs
+            )
+        elif plot_type == "plotly":
+            out_path = os.path.basename(summary_csv).replace(".csv", ".html")
             out_path = os.path.join(out_dir, out_path)
-            splt.scatter_plotly(value, cmap=cmap.capitalize(),
-                                out_path=out_path, **kwargs)
+            splt.scatter_plotly(
+                value, cmap=cmap.capitalize(), out_path=out_path, **kwargs
+            )
         else:
-            msg = ("plot_type must be 'plot' or 'plotly' but {} was given"
-                   .format(plot_type))
+            msg = (
+                "plot_type must be 'plot' or 'plotly' but {} was given".format(
+                    plot_type
+                )
+            )
             logger.error(msg)
             raise ValueError(msg)
 
     @classmethod
-    def scatter_all(cls, summary_csv, out_dir, plot_type='plotly',
-                    cmap='viridis', **kwargs):
+    def scatter_all(
+        cls, summary_csv, out_dir, plot_type="plotly", cmap="viridis", **kwargs
+    ):
         """
         Create scatter plot for all summary stats in summary table and save to
         out_dir
 
         Parameters
         ----------
         summary_csv : str
@@ -670,32 +715,37 @@
         cmap : str, optional
             Colormap name, by default 'viridis'
         kwargs : dict
             Additional plotting kwargs
         """
         splt = cls(summary_csv)
         splt._data = splt.summary.select_dtypes(include=np.number)
-        datasets = [c for c in splt.summary.columns
-                    if not c.startswith(('lat', 'lon'))]
+        datasets = [
+            c for c in splt.summary.columns if not c.startswith(("lat", "lon"))
+        ]
 
         for value in datasets:
-            if plot_type == 'plot':
-                out_path = '_{}.png'.format(value)
-                out_path = \
-                    os.path.basename(summary_csv).replace('.csv', out_path)
+            if plot_type == "plot":
+                out_path = "_{}.png".format(value)
+                out_path = os.path.basename(summary_csv).replace(
+                    ".csv", out_path
+                )
                 out_path = os.path.join(out_dir, out_path)
-                splt.scatter_plot(value, cmap=cmap.lower(), out_path=out_path,
-                                  **kwargs)
-            elif plot_type == 'plotly':
-                out_path = '_{}.html'.format(value)
-                out_path = \
-                    os.path.basename(summary_csv).replace('.csv', out_path)
+                splt.scatter_plot(
+                    value, cmap=cmap.lower(), out_path=out_path, **kwargs
+                )
+            elif plot_type == "plotly":
+                out_path = "_{}.html".format(value)
+                out_path = os.path.basename(summary_csv).replace(
+                    ".csv", out_path
+                )
                 out_path = os.path.join(out_dir, out_path)
-                splt.scatter_plotly(value, cmap=cmap.capitalize(),
-                                    out_path=out_path, **kwargs)
+                splt.scatter_plotly(
+                    value, cmap=cmap.capitalize(), out_path=out_path, **kwargs
+                )
             else:
                 msg = ("plot_type must be 'plot' or 'plotly' but {} was given"
                        .format(plot_type))
                 logger.error(msg)
                 raise ValueError(msg)
 
 
@@ -731,107 +781,116 @@
 
         Returns
         -------
         list
         """
         return list(self.sc_table.columns)
 
-    def _extract_sc_data(self, lcoe='mean_lcoe'):
+    def _extract_sc_data(self, lcoe=SupplyCurveField.MEAN_LCOE):
         """
         Extract supply curve data
 
         Parameters
         ----------
         lcoe : str, optional
-            LCOE value to use for supply curve, by default 'mean_lcoe'
+            LCOE value to use for supply curve,
+            by default :obj:`SupplyCurveField.MEAN_LCOE`
 
         Returns
         -------
         sc_df : pandas.DataFrame
             Supply curve data
         """
-        values = ['capacity', lcoe]
+        values = [SupplyCurveField.CAPACITY, lcoe]
         self._check_value(self.sc_table, values, scatter=False)
         sc_df = self.sc_table[values].sort_values(lcoe)
-        sc_df['cumulative_capacity'] = sc_df['capacity'].cumsum()
+        sc_df['cumulative_capacity'] = (
+            sc_df[SupplyCurveField.CAPACITY].cumsum()
+        )
 
         return sc_df
 
-    def supply_curve_plot(self, lcoe='mean_lcoe', out_path=None, **kwargs):
+    def supply_curve_plot(self, lcoe=SupplyCurveField.MEAN_LCOE, out_path=None,
+                          **kwargs):
         """
         Plot supply curve (cumulative capacity vs lcoe) using seaborn.scatter
 
         Parameters
         ----------
         lcoe : str, optional
-            LCOE value to plot, by default 'mean_lcoe'
+            LCOE value to plot, by default :obj:`SupplyCurveField.MEAN_LCOE`
         out_path : str, optional
             File path to save plot to, by default None
         kwargs : dict
             Additional kwargs for plotting.dataframes.df_scatter
         """
         sc_df = self._extract_sc_data(lcoe=lcoe)
-        mplt.df_scatter(sc_df, x='cumulative_capacity', y=lcoe,
-                        filename=out_path, **kwargs)
+        mplt.df_scatter(
+            sc_df, x="cumulative_capacity", y=lcoe, filename=out_path, **kwargs
+        )
 
-    def supply_curve_plotly(self, lcoe='mean_lcoe', out_path=None, **kwargs):
+    def supply_curve_plotly(self, lcoe=SupplyCurveField.MEAN_LCOE,
+                            out_path=None, **kwargs):
         """
         Plot supply curve (cumulative capacity vs lcoe) using plotly
 
         Parameters
         ----------
         lcoe : str, optional
-            LCOE value to plot, by default 'mean_lcoe'
+            LCOE value to plot, by default SupplyCurveField.MEAN_LCOE
         out_path : str, optional
             File path to save plot to, can be a .html or static image,
             by default None
         kwargs : dict
             Additional kwargs for plotly.express.scatter
         """
         sc_df = self._extract_sc_data(lcoe=lcoe)
-        fig = px.scatter(sc_df, x='cumulative_capacity', y=lcoe, **kwargs)
+        fig = px.scatter(sc_df, x="cumulative_capacity", y=lcoe, **kwargs)
         fig.update_layout(font=dict(family="Arial", size=18, color="black"))
 
         if out_path is not None:
             self._save_plotly(fig, out_path)
 
         fig.show()
 
     @classmethod
-    def plot(cls, sc_table, out_dir, plot_type='plotly', lcoe='mean_lcoe',
-             **kwargs):
+    def plot(cls, sc_table, out_dir, plot_type='plotly',
+             lcoe=SupplyCurveField.MEAN_LCOE, **kwargs):
         """
         Create supply curve plot from supply curve table using lcoe value
         and save to out_dir
 
         Parameters
         ----------
         sc_table : str
             Path to .csv file containing Supply Curve table
         out_dir : str
             Output directory to save plots to
         plot_type : str, optional
             plot_type of plot to create 'plot' or 'plotly', by default 'plotly'
         lcoe : str, optional
-            LCOE value to plot, by default 'mean_lcoe'
+            LCOE value to plot, by default :obj:`SupplyCurveField.MEAN_LCOE`
         kwargs : dict
             Additional plotting kwargs
         """
         splt = cls(sc_table)
-        if plot_type == 'plot':
-            out_path = os.path.basename(sc_table).replace('.csv', '.png')
+        if plot_type == "plot":
+            out_path = os.path.basename(sc_table).replace(".csv", ".png")
             out_path = os.path.join(out_dir, out_path)
             splt.supply_curve_plot(lcoe=lcoe, out_path=out_path, **kwargs)
-        elif plot_type == 'plotly':
-            out_path = os.path.basename(sc_table).replace('.csv', '.html')
+        elif plot_type == "plotly":
+            out_path = os.path.basename(sc_table).replace(".csv", ".html")
             out_path = os.path.join(out_dir, out_path)
             splt.supply_curve_plotly(lcoe=lcoe, out_path=out_path, **kwargs)
         else:
-            msg = ("plot_type must be 'plot' or 'plotly' but {} was given"
-                   .format(plot_type))
+            msg = (
+                "plot_type must be 'plot' or 'plotly' but {} was given".format(
+                    plot_type
+                )
+            )
             logger.error(msg)
             raise ValueError(msg)
 
 
 class ExclusionsMask(PlotBase):
     """
     Plot Exclusions mask as a heat map data for QA/QC
@@ -875,16 +934,17 @@
         if isinstance(excl_mask, str):
             excl_mask = np.load(excl_mask)
         elif not isinstance(excl_mask, np.ndarray):
             raise ValueError("excl_mask must be a .npy file or an ndarray")
 
         return excl_mask
 
-    def exclusions_plot(self, cmap='Viridis', plot_step=100, out_path=None,
-                        **kwargs):
+    def exclusions_plot(
+        self, cmap="Viridis", plot_step=100, out_path=None, **kwargs
+    ):
         """
         Plot exclusions mask as a seaborn heatmap
 
         Parameters
         ----------
         cmap : str | px.color, optional
             Continuous color scale to use, by default 'Viridis'
@@ -892,19 +952,24 @@
             Step between points to plot
         out_path : str, optional
             File path to save plot to, can be a .html or static image,
             by default None
         kwargs : dict
             Additional kwargs for plotting.colormaps.heatmap_plot
         """
-        mplt.heatmap_plot(self.mask[::plot_step, ::plot_step], cmap=cmap,
-                          filename=out_path, **kwargs)
-
-    def exclusions_plotly(self, cmap='Viridis', plot_step=100, out_path=None,
-                          **kwargs):
+        mplt.heatmap_plot(
+            self.mask[::plot_step, ::plot_step],
+            cmap=cmap,
+            filename=out_path,
+            **kwargs,
+        )
+
+    def exclusions_plotly(
+        self, cmap="Viridis", plot_step=100, out_path=None, **kwargs
+    ):
         """
         Plot exclusions mask as a plotly heatmap
 
         Parameters
         ----------
         cmap : str | px.color, optional
             Continuous color scale to use, by default 'Viridis'
@@ -912,26 +977,36 @@
             Step between points to plot
         out_path : str, optional
             File path to save plot to, can be a .html or static image,
             by default None
         kwargs : dict
             Additional kwargs for plotly.express.imshow
         """
-        fig = px.imshow(self.mask[::plot_step, ::plot_step],
-                        color_continuous_scale=cmap, **kwargs)
+        fig = px.imshow(
+            self.mask[::plot_step, ::plot_step],
+            color_continuous_scale=cmap,
+            **kwargs,
+        )
         fig.update_layout(font=dict(family="Arial", size=18, color="black"))
 
         if out_path is not None:
             SummaryPlots._save_plotly(fig, out_path)
 
         fig.show()
 
     @classmethod
-    def plot(cls, mask, out_dir, plot_type='plotly', cmap='Viridis',
-             plot_step=100, **kwargs):
+    def plot(
+        cls,
+        mask,
+        out_dir,
+        plot_type="plotly",
+        cmap="Viridis",
+        plot_step=100,
+        **kwargs,
+    ):
         """
         Plot exclusions mask and save to out_dir
 
         Parameters
         ----------
         mask : ndarray
             ndarray of final exclusions mask
@@ -943,26 +1018,33 @@
             Colormap name, by default 'viridis'
         plot_step : int
             Step between points to plot
         kwargs : dict
             Additional plotting kwargs
         """
         excl_mask = cls(mask)
-        if plot_type == 'plot':
-            out_path = 'exclusions_mask.png'
+        if plot_type == "plot":
+            out_path = "exclusions_mask.png"
             out_path = os.path.join(out_dir, out_path)
-            excl_mask.exclusions_plot(cmap=cmap.lower(),
-                                      plot_step=plot_step,
-                                      out_path=out_path,
-                                      **kwargs)
-        elif plot_type == 'plotly':
-            out_path = 'exclusions_mask.html'
+            excl_mask.exclusions_plot(
+                cmap=cmap.lower(),
+                plot_step=plot_step,
+                out_path=out_path,
+                **kwargs,
+            )
+        elif plot_type == "plotly":
+            out_path = "exclusions_mask.html"
             out_path = os.path.join(out_dir, out_path)
-            excl_mask.exclusions_plotly(cmap=cmap.capitalize(),
-                                        plot_step=plot_step,
-                                        out_path=out_path,
-                                        **kwargs)
+            excl_mask.exclusions_plotly(
+                cmap=cmap.capitalize(),
+                plot_step=plot_step,
+                out_path=out_path,
+                **kwargs,
+            )
         else:
-            msg = ("plot_type must be 'plot' or 'plotly' but {} was given"
-                   .format(plot_type))
+            msg = (
+                "plot_type must be 'plot' or 'plotly' but {} was given".format(
+                    plot_type
+                )
+            )
             logger.error(msg)
             raise ValueError(msg)
```

### Comparing `NREL-reV-0.8.7/reV/rep_profiles/cli_rep_profiles.py` & `NREL-reV-0.8.9/reV/rep_profiles/cli_rep_profiles.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/rep_profiles/rep_profiles.py` & `NREL-reV-0.8.9/reV/rep_profiles/rep_profiles.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # -*- coding: utf-8 -*-
 """Representative profile extraction utilities.
 
 Created on Thu Oct 31 12:49:23 2019
 
 @author: gbuster
 """
-from abc import ABC, abstractmethod
-from concurrent.futures import as_completed
-from copy import deepcopy
+import contextlib
 import json
 import logging
-import numpy as np
 import os
-import pandas as pd
-from scipy import stats
+from abc import ABC, abstractmethod
+from concurrent.futures import as_completed
+from copy import deepcopy
 from warnings import warn
 
-
-from reV.handlers.outputs import Outputs
-from reV.utilities.exceptions import FileInputError, DataShapeError
-from reV.utilities import log_versions
-
+import numpy as np
+import pandas as pd
 from rex.resource import Resource
 from rex.utilities.execution import SpawnProcessPool
 from rex.utilities.loggers import log_mem
 from rex.utilities.utilities import parse_year, to_records_array
+from scipy import stats
+
+from reV.handlers.outputs import Outputs
+from reV.utilities import ResourceMetaField, SupplyCurveField, log_versions
+from reV.utilities.exceptions import DataShapeError, FileInputError
 
 logger = logging.getLogger(__name__)
 
 
 class RepresentativeMethods:
     """Class for organizing the methods to determine representative-ness"""
 
-    def __init__(self, profiles, weights=None, rep_method='meanoid',
-                 err_method='rmse'):
+    def __init__(
+        self, profiles, weights=None, rep_method="meanoid", err_method="rmse"
+    ):
         """
         Parameters
         ----------
         profiles : np.ndarray
             (time, sites) timeseries array of cf profile data.
         weights : np.ndarray | list
             1D array of weighting factors (multiplicative) for profiles.
@@ -57,38 +58,43 @@
 
     def _parse_weights(self):
         """Parse the weights attribute. Check shape and make np.array."""
         if isinstance(self._weights, (list, tuple)):
             self._weights = np.array(self._weights)
 
         if self._weights is not None:
-            emsg = ('Weighting factors array of length {} does not match '
-                    'profiles of shape {}'
-                    .format(len(self._weights), self._profiles.shape[1]))
+            emsg = (
+                "Weighting factors array of length {} does not match "
+                "profiles of shape {}".format(
+                    len(self._weights), self._profiles.shape[1]
+                )
+            )
             assert len(self._weights) == self._profiles.shape[1], emsg
 
     @property
     def rep_methods(self):
         """Lookup table of representative methods"""
-        methods = {'mean': self.meanoid,
-                   'meanoid': self.meanoid,
-                   'median': self.medianoid,
-                   'medianoid': self.medianoid,
-                   }
+        methods = {
+            "mean": self.meanoid,
+            "meanoid": self.meanoid,
+            "median": self.medianoid,
+            "medianoid": self.medianoid,
+        }
 
         return methods
 
     @property
     def err_methods(self):
         """Lookup table of error methods"""
-        methods = {'mbe': self.mbe,
-                   'mae': self.mae,
-                   'rmse': self.rmse,
-                   None: None,
-                   }
+        methods = {
+            "mbe": self.mbe,
+            "mae": self.mae,
+            "rmse": self.rmse,
+            None: None,
+        }
 
         return methods
 
     @staticmethod
     def nargmin(arr, n):
         """Get the index of the Nth min value in arr.
 
@@ -101,15 +107,15 @@
             If n is 1, this returns the location of the 2nd min value in arr.
 
         Returns
         -------
         i : int
             Location of the Nth min value in arr.
         """
-        return arr.argsort()[:(n + 1)][-1]
+        return arr.argsort()[: (n + 1)][-1]
 
     @staticmethod
     def meanoid(profiles, weights=None):
         """Find the mean profile across all sites.
 
         Parameters
         ----------
@@ -237,16 +243,22 @@
         rmse **= 2
         rmse = np.sqrt(np.mean(rmse, axis=0))
         i_rep = cls.nargmin(rmse, i_profile)
 
         return profiles[:, i_rep], i_rep
 
     @classmethod
-    def run(cls, profiles, weights=None, rep_method='meanoid',
-            err_method='rmse', n_profiles=1):
+    def run(
+        cls,
+        profiles,
+        weights=None,
+        rep_method="meanoid",
+        err_method="rmse",
+        n_profiles=1,
+    ):
         """Run representative profile methods.
 
         Parameters
         ----------
         profiles : np.ndarray
             (time, sites) timeseries array of cf profile data.
         weights : np.ndarray | list
@@ -266,16 +278,20 @@
         profiles : np.ndarray
             (time, n_profiles) array for the most representative profile(s)
         i_reps : list | None
             List (length of n_profiles) with column Index in profiles of the
             representative profile(s). If err_method is None, this value is
             also set to None.
         """
-        inst = cls(profiles, weights=weights, rep_method=rep_method,
-                   err_method=err_method)
+        inst = cls(
+            profiles,
+            weights=weights,
+            rep_method=rep_method,
+            err_method=err_method,
+        )
 
         if inst._weights is not None:
             baseline = inst._rep_method(inst._profiles, weights=inst._weights)
         else:
             baseline = inst._rep_method(inst._profiles)
 
         if err_method is None:
@@ -295,19 +311,20 @@
 
         return profiles, i_reps
 
 
 class RegionRepProfile:
     """Framework to handle rep profile for one resource region"""
 
-    RES_GID_COL = 'res_gids'
-    GEN_GID_COL = 'gen_gids'
+    RES_GID_COL = SupplyCurveField.RES_GIDS
+    GEN_GID_COL = SupplyCurveField.GEN_GIDS
 
     def __init__(self, gen_fpath, rev_summary, cf_dset='cf_profile',
-                 rep_method='meanoid', err_method='rmse', weight='gid_counts',
+                 rep_method='meanoid', err_method='rmse',
+                 weight=SupplyCurveField.GID_COUNTS,
                  n_profiles=1):
         """
         Parameters
         ----------
         gen_fpath : str
             Filepath to reV gen output file to extract "cf_profile" from.
         rev_summary : pd.DataFrame
@@ -351,46 +368,54 @@
     def _init_profiles_weights(self):
         """Initialize the base source profiles and weight arrays"""
         gen_gids = self._get_region_attr(self._rev_summary, self.GEN_GID_COL)
         res_gids = self._get_region_attr(self._rev_summary, self.RES_GID_COL)
 
         self._weights = np.ones(len(res_gids))
         if self._weight is not None:
-            self._weights = self._get_region_attr(self._rev_summary,
-                                                  self._weight)
+            self._weights = self._get_region_attr(
+                self._rev_summary, self._weight
+            )
 
-        df = pd.DataFrame({self.GEN_GID_COL: gen_gids,
-                           self.RES_GID_COL: res_gids,
-                           'weights': self._weights})
+        df = pd.DataFrame(
+            {
+                self.GEN_GID_COL: gen_gids,
+                self.RES_GID_COL: res_gids,
+                "weights": self._weights,
+            }
+        )
         df = df.sort_values(self.RES_GID_COL)
         self._gen_gids = df[self.GEN_GID_COL].values
         self._res_gids = df[self.RES_GID_COL].values
         if self._weight is not None:
-            self._weights = df['weights'].values
+            self._weights = df["weights"].values
         else:
             self._weights = None
 
         with Resource(self._gen_fpath) as res:
             meta = res.meta
 
-            assert 'gid' in meta
-            source_res_gids = meta['gid'].values
+            assert ResourceMetaField.GID in meta
+            source_res_gids = meta[ResourceMetaField.GID].values
             msg = ('Resource gids from "gid" column in meta data from "{}" '
                    'must be sorted! reV generation should always be run with '
                    'sequential project points.'.format(self._gen_fpath))
             assert np.all(source_res_gids[:-1] <= source_res_gids[1:]), msg
 
             missing = set(self._res_gids) - set(source_res_gids)
-            msg = ('The following resource gids were found in the rev summary '
-                   'supply curve file but not in the source generation meta '
-                   'data: {}'.format(missing))
+            msg = (
+                "The following resource gids were found in the rev summary "
+                "supply curve file but not in the source generation meta "
+                "data: {}".format(missing)
+            )
             assert not any(missing), msg
 
-            unique_res_gids, u_idxs = np.unique(self._res_gids,
-                                                return_inverse=True)
+            unique_res_gids, u_idxs = np.unique(
+                self._res_gids, return_inverse=True
+            )
             iloc = np.where(np.isin(source_res_gids, unique_res_gids))[0]
             self._source_profiles = res[self._cf_dset, :, iloc[u_idxs]]
 
     @property
     def source_profiles(self):
         """Retrieve the cf profile array from the source generation h5 file.
 
@@ -437,88 +462,95 @@
             will be unpacked.
         """
         data = rev_summary[attr_name].values.tolist()
 
         if any(data):
             if isinstance(data[0], str):
                 # pylint: disable=simplifiable-condition
-                if ('[' and ']' in data[0]) or ('(' and ')' in data[0]):
+                if ("[" and "]" in data[0]) or ("(" and ")" in data[0]):
                     data = [json.loads(s) for s in data]
 
             if isinstance(data[0], (list, tuple)):
                 data = [a for b in data for a in b]
 
         return data
 
     def _run_rep_methods(self):
         """Run the representative profile methods to find the meanoid/medianoid
         profile and find the profiles most similar."""
 
-        if self.weights is not None:
-            if len(self.weights) != self.source_profiles.shape[1]:
-                e = ('Weights column "{}" resulted in {} weight scalars '
-                     'which doesnt match gid column which yields '
-                     'profiles with shape {}.'
-                     .format(self._weight, len(self.weights),
-                             self.source_profiles.shape))
-                logger.debug('Gids from column "res_gids" with len {}: {}'
-                             .format(len(self._res_gids), self._res_gids))
-                logger.debug('Weights from column "{}" with len {}: {}'
-                             .format(self._weight, len(self.weights),
-                                     self.weights))
-                logger.error(e)
-                raise DataShapeError(e)
+        num_profiles = self.source_profiles.shape[1]
+        bad_data_shape = (self.weights is not None
+                          and len(self.weights) != num_profiles)
+        if bad_data_shape:
+            e = ('Weights column "{}" resulted in {} weight scalars '
+                 'which doesnt match gid column which yields '
+                 'profiles with shape {}.'
+                 .format(self._weight, len(self.weights),
+                         self.source_profiles.shape))
+            logger.debug('Gids from column "res_gids" with len {}: {}'
+                         .format(len(self._res_gids), self._res_gids))
+            logger.debug('Weights from column "{}" with len {}: {}'
+                         .format(self._weight, len(self.weights),
+                                 self.weights))
+            logger.error(e)
+            raise DataShapeError(e)
 
         self._profiles, self._i_reps = RepresentativeMethods.run(
-            self.source_profiles, weights=self.weights,
-            rep_method=self._rep_method, err_method=self._err_method,
-            n_profiles=self._n_profiles)
+            self.source_profiles,
+            weights=self.weights,
+            rep_method=self._rep_method,
+            err_method=self._err_method,
+            n_profiles=self._n_profiles,
+        )
 
-    @property
+    @ property
     def rep_profiles(self):
         """Get the representative profiles of this region."""
         if self._profiles is None:
             self._run_rep_methods()
 
         return self._profiles
 
-    @property
+    @ property
     def i_reps(self):
         """Get the representative profile index(es) of this region."""
         if self._i_reps is None:
             self._run_rep_methods()
 
         return self._i_reps
 
-    @property
+    @ property
     def rep_gen_gids(self):
         """Get the representative profile gen gids of this region."""
         gids = self._gen_gids
         if self.i_reps[0] is None:
             rep_gids = None
         else:
             rep_gids = [gids[i] for i in self.i_reps]
 
         return rep_gids
 
-    @property
+    @ property
     def rep_res_gids(self):
         """Get the representative profile resource gids of this region."""
         gids = self._res_gids
         if self.i_reps[0] is None or gids is None:
             rep_gids = [None]
         else:
             rep_gids = [gids[i] for i in self.i_reps]
 
         return rep_gids
 
-    @classmethod
+    @ classmethod
     def get_region_rep_profile(cls, gen_fpath, rev_summary,
-                               cf_dset='cf_profile', rep_method='meanoid',
-                               err_method='rmse', weight='gid_counts',
+                               cf_dset='cf_profile',
+                               rep_method='meanoid',
+                               err_method='rmse',
+                               weight=SupplyCurveField.GID_COUNTS,
                                n_profiles=1):
         """Class method for parallelization of rep profile calc.
 
         Parameters
         ----------
         gen_fpath : str
             Filepath to reV gen output file to extract "cf_profile" from.
@@ -550,27 +582,34 @@
         i_rep : list
             Column Index in profiles of the representative profile(s).
         gen_gid_reps : list
             Generation gid(s) of the representative profile(s).
         res_gid_reps : list
             Resource gid(s) of the representative profile(s).
         """
-        r = cls(gen_fpath, rev_summary, cf_dset=cf_dset,
-                rep_method=rep_method, err_method=err_method, weight=weight,
-                n_profiles=n_profiles)
+        r = cls(
+            gen_fpath,
+            rev_summary,
+            cf_dset=cf_dset,
+            rep_method=rep_method,
+            err_method=err_method,
+            weight=weight,
+            n_profiles=n_profiles,
+        )
 
         return r.rep_profiles, r.i_reps, r.rep_gen_gids, r.rep_res_gids
 
 
 class RepProfilesBase(ABC):
     """Abstract utility framework for representative profile run classes."""
 
     def __init__(self, gen_fpath, rev_summary, reg_cols=None,
-                 cf_dset='cf_profile', rep_method='meanoid', err_method='rmse',
-                 weight='gid_counts', n_profiles=1):
+                 cf_dset='cf_profile', rep_method='meanoid',
+                 err_method='rmse', weight=SupplyCurveField.GID_COUNTS,
+                 n_profiles=1):
         """
         Parameters
         ----------
         gen_fpath : str
             Filepath to reV gen output file to extract "cf_profile" from.
         rev_summary : str | pd.DataFrame
             Aggregated rev supply curve summary file. Str filepath or full df.
@@ -593,26 +632,34 @@
             Column in rev_summary used to apply weighted mean to profiles.
             The supply curve table data in the weight column should have
             weight values corresponding to the res_gids in the same row.
         n_profiles : int
             Number of representative profiles to save to fout.
         """
 
-        logger.info('Running rep profiles with gen_fpath: "{}"'
-                    .format(gen_fpath))
-        logger.info('Running rep profiles with rev_summary: "{}"'
-                    .format(rev_summary))
-        logger.info('Running rep profiles with region columns: "{}"'
-                    .format(reg_cols))
-        logger.info('Running rep profiles with representative method: "{}"'
-                    .format(rep_method))
-        logger.info('Running rep profiles with error method: "{}"'
-                    .format(err_method))
-        logger.info('Running rep profiles with weight factor: "{}"'
-                    .format(weight))
+        logger.info(
+            'Running rep profiles with gen_fpath: "{}"'.format(gen_fpath)
+        )
+        logger.info(
+            'Running rep profiles with rev_summary: "{}"'.format(rev_summary)
+        )
+        logger.info(
+            'Running rep profiles with region columns: "{}"'.format(reg_cols)
+        )
+        logger.info(
+            'Running rep profiles with representative method: "{}"'.format(
+                rep_method
+            )
+        )
+        logger.info(
+            'Running rep profiles with error method: "{}"'.format(err_method)
+        )
+        logger.info(
+            'Running rep profiles with weight factor: "{}"'.format(weight)
+        )
 
         self._weight = weight
         self._n_profiles = n_profiles
         self._cf_dset = cf_dset
         self._gen_fpath = gen_fpath
         self._reg_cols = reg_cols
 
@@ -626,15 +673,15 @@
         self._check_rev_gen(gen_fpath, cf_dset, self._rev_summary)
         self._time_index = None
         self._meta = None
         self._profiles = None
         self._rep_method = rep_method
         self._err_method = err_method
 
-    @staticmethod
+    @ staticmethod
     def _parse_rev_summary(rev_summary):
         """Extract, parse, and check the rev summary table.
 
         Parameters
         ----------
         rev_summary : str | pd.DataFrame
             Aggregated rev supply curve summary file. Str filepath or full df.
@@ -646,57 +693,56 @@
         rev_summary : pd.DataFrame
             Aggregated rev supply curve summary file. Full df.
             Must include "res_gids", "gen_gids", and the "weight" column (if
             weight is not None)
         """
 
         if isinstance(rev_summary, str):
-            if os.path.exists(rev_summary) and rev_summary.endswith('.csv'):
+            if os.path.exists(rev_summary) and rev_summary.endswith(".csv"):
                 rev_summary = pd.read_csv(rev_summary)
-            elif os.path.exists(rev_summary) and rev_summary.endswith('.json'):
+            elif os.path.exists(rev_summary) and rev_summary.endswith(".json"):
                 rev_summary = pd.read_json(rev_summary)
             else:
-                e = 'Could not parse reV summary file: {}'.format(rev_summary)
+                e = "Could not parse reV summary file: {}".format(rev_summary)
                 logger.error(e)
                 raise FileInputError(e)
         elif not isinstance(rev_summary, pd.DataFrame):
-            e = ('Bad input dtype for rev_summary input: {}'
-                 .format(type(rev_summary)))
+            e = "Bad input dtype for rev_summary input: {}".format(
+                type(rev_summary)
+            )
             logger.error(e)
             raise TypeError(e)
 
         return rev_summary
 
-    @staticmethod
+    @ staticmethod
     def _check_req_cols(df, cols):
         """Check a dataframe for required columns.
 
         Parameters
         ----------
         df : pd.DataFrame
             Dataframe to check columns.
         cols : str | list | tuple
             Required columns in df.
         """
         if cols is not None:
             if isinstance(cols, str):
                 cols = [cols]
 
-            missing = []
-            for c in cols:
-                if c not in df:
-                    missing.append(c)
+            missing = [c for c in cols if c not in df]
 
             if any(missing):
-                e = ('Column labels not found in rev_summary table: {}'
-                     .format(missing))
+                e = "Column labels not found in rev_summary table: {}".format(
+                    missing
+                )
                 logger.error(e)
                 raise KeyError(e)
 
-    @staticmethod
+    @ staticmethod
     def _check_rev_gen(gen_fpath, cf_dset, rev_summary):
         """Check rev gen file for requisite datasets.
 
         Parameters
         ----------
         gen_fpath : str
             Filepath to reV gen output file to extract "cf_profile" from.
@@ -706,85 +752,96 @@
             Aggregated rev supply curve summary file. Full df.
             Must include "res_gids", "gen_gids", and the "weight" column (if
             weight is not None)
         """
         with Resource(gen_fpath) as res:
             dsets = res.datasets
             if cf_dset not in dsets:
-                raise KeyError('reV gen file needs to have "{}" '
-                               'dataset to calculate representative profiles!'
-                               .format(cf_dset))
-
-            if 'time_index' not in str(dsets):
-                raise KeyError('reV gen file needs to have "time_index" '
-                               'dataset to calculate representative profiles!')
+                raise KeyError(
+                    'reV gen file needs to have "{}" '
+                    "dataset to calculate representative profiles!".format(
+                        cf_dset
+                    )
+                )
+
+            if "time_index" not in str(dsets):
+                raise KeyError(
+                    'reV gen file needs to have "time_index" '
+                    "dataset to calculate representative profiles!"
+                )
 
             shape = res.get_dset_properties(cf_dset)[0]
 
         if len(rev_summary) > shape[1]:
-            msg = ('WARNING: reV SC summary table has {} sc points and CF '
-                   'dataset "{}" has {} profiles. There should never be more '
-                   'SC points than CF profiles.'
-                   .format(len(rev_summary), cf_dset, shape[1]))
+            msg = (
+                "WARNING: reV SC summary table has {} sc points and CF "
+                'dataset "{}" has {} profiles. There should never be more '
+                "SC points than CF profiles.".format(
+                    len(rev_summary), cf_dset, shape[1]
+                )
+            )
             logger.warning(msg)
             warn(msg)
 
     def _init_profiles(self):
         """Initialize the output rep profiles attribute."""
-        self._profiles = {k: np.zeros((len(self.time_index),
-                                       len(self.meta)),
-                                      dtype=np.float32)
-                          for k in range(self._n_profiles)}
+        self._profiles = {
+            k: np.zeros(
+                (len(self.time_index), len(self.meta)), dtype=np.float32
+            )
+            for k in range(self._n_profiles)
+        }
 
-    @property
+    @ property
     def time_index(self):
         """Get the time index for the rep profiles.
 
         Returns
         -------
         time_index : pd.datetimeindex
             Time index sourced from the reV gen file.
         """
         if self._time_index is None:
             with Resource(self._gen_fpath) as res:
-                ds = 'time_index'
-                if parse_year(self._cf_dset, option='bool'):
-                    year = parse_year(self._cf_dset, option='raise')
-                    ds += '-{}'.format(year)
+                ds = "time_index"
+                if parse_year(self._cf_dset, option="bool"):
+                    year = parse_year(self._cf_dset, option="raise")
+                    ds += "-{}".format(year)
 
                 self._time_index = res._get_time_index(ds, slice(None))
 
         return self._time_index
 
-    @property
+    @ property
     def meta(self):
         """Meta data for the representative profiles.
 
         Returns
         -------
         meta : pd.DataFrame
             Meta data for the representative profiles. At the very least,
             this has columns for the region and res class.
         """
         return self._meta
 
-    @property
+    @ property
     def profiles(self):
         """Get the arrays of representative CF profiles corresponding to meta.
 
         Returns
         -------
         profiles : dict
             dict of n_profile-keyed arrays with shape (time, n) for the
             representative profiles for each region.
         """
         return self._profiles
 
-    def _init_h5_out(self, fout, save_rev_summary=True,
-                     scaled_precision=False):
+    def _init_h5_out(
+        self, fout, save_rev_summary=True, scaled_precision=False
+    ):
         """Initialize an output h5 file for n_profiles
 
         Parameters
         ----------
         fout : str
             None or filepath to output h5 file.
         save_rev_summary : bool
@@ -795,102 +852,114 @@
         dsets = []
         shapes = {}
         attrs = {}
         chunks = {}
         dtypes = {}
 
         for i in range(self._n_profiles):
-            dset = 'rep_profiles_{}'.format(i)
+            dset = "rep_profiles_{}".format(i)
             dsets.append(dset)
             shapes[dset] = self.profiles[0].shape
             chunks[dset] = None
 
             if scaled_precision:
-                attrs[dset] = {'scale_factor': 1000}
+                attrs[dset] = {"scale_factor": 1000}
                 dtypes[dset] = np.uint16
             else:
                 attrs[dset] = None
                 dtypes[dset] = self.profiles[0].dtype
 
         meta = self.meta.copy()
         for c in meta.columns:
-            try:
+            with contextlib.suppress(ValueError):
                 meta[c] = pd.to_numeric(meta[c])
-            except ValueError:
-                pass
 
-        Outputs.init_h5(fout, dsets, shapes, attrs, chunks, dtypes,
-                        meta, time_index=self.time_index)
+        Outputs.init_h5(
+            fout,
+            dsets,
+            shapes,
+            attrs,
+            chunks,
+            dtypes,
+            meta,
+            time_index=self.time_index,
+        )
 
         if save_rev_summary:
-            with Outputs(fout, mode='a') as out:
+            with Outputs(fout, mode="a") as out:
                 rev_sum = to_records_array(self._rev_summary)
-                out._create_dset('rev_summary', rev_sum.shape,
-                                 rev_sum.dtype, data=rev_sum)
+                out._create_dset(
+                    "rev_summary", rev_sum.shape, rev_sum.dtype, data=rev_sum
+                )
 
     def _write_h5_out(self, fout, save_rev_summary=True):
         """Write profiles and meta to an output file.
 
         Parameters
         ----------
         fout : str
             None or filepath to output h5 file.
         save_rev_summary : bool
             Flag to save full reV SC table to rep profile output.
         scaled_precision : bool
             Flag to scale cf_profiles by 1000 and save as uint16.
         """
-        with Outputs(fout, mode='a') as out:
-
-            if 'rev_summary' in out.datasets and save_rev_summary:
+        with Outputs(fout, mode="a") as out:
+            if "rev_summary" in out.datasets and save_rev_summary:
                 rev_sum = to_records_array(self._rev_summary)
-                out['rev_summary'] = rev_sum
+                out["rev_summary"] = rev_sum
 
             for i in range(self._n_profiles):
-                dset = 'rep_profiles_{}'.format(i)
+                dset = "rep_profiles_{}".format(i)
                 out[dset] = self.profiles[i]
 
-    def save_profiles(self, fout, save_rev_summary=True,
-                      scaled_precision=False):
+    def save_profiles(
+        self, fout, save_rev_summary=True, scaled_precision=False
+    ):
         """Initialize fout and save profiles.
 
         Parameters
         ----------
         fout : str
             None or filepath to output h5 file.
         save_rev_summary : bool
             Flag to save full reV SC table to rep profile output.
         scaled_precision : bool
             Flag to scale cf_profiles by 1000 and save as uint16.
         """
 
-        self._init_h5_out(fout, save_rev_summary=save_rev_summary,
-                          scaled_precision=scaled_precision)
+        self._init_h5_out(
+            fout,
+            save_rev_summary=save_rev_summary,
+            scaled_precision=scaled_precision,
+        )
         self._write_h5_out(fout, save_rev_summary=save_rev_summary)
 
-    @abstractmethod
+    @ abstractmethod
     def _run_serial(self):
         """Abstract method for serial run method."""
 
-    @abstractmethod
+    @ abstractmethod
     def _run_parallel(self):
         """Abstract method for parallel run method."""
 
-    @abstractmethod
+    @ abstractmethod
     def run(self):
         """Abstract method for generic run method."""
 
 
 class RepProfiles(RepProfilesBase):
     """RepProfiles"""
 
-    def __init__(self, gen_fpath, rev_summary, reg_cols, cf_dset='cf_profile',
-                 rep_method='meanoid', err_method='rmse', weight='gid_counts',
+    def __init__(self, gen_fpath, rev_summary, reg_cols,
+                 cf_dset='cf_profile',
+                 rep_method='meanoid', err_method='rmse',
+                 weight=SupplyCurveField.GID_COUNTS,
                  n_profiles=1, aggregate_profiles=False):
-        """reV rep profiles class.
+        """ReV rep profiles class.
 
         ``reV`` rep profiles compute representative generation profiles
         for each supply curve point output by ``reV`` supply curve
         aggregation. Representative profiles can either be a spatial
         aggregation of generation profiles or actual generation profiles
         that most closely resemble an aggregated profile (selected based
         on an error metric).
@@ -973,74 +1042,86 @@
                are weighted equally. For example, if you have a 64x64
                supply curve point, and one generation profile takes up
                4095 (99.98%) 90m cells while a second generation profile
                takes up only one 90m cell (0.02%), they will contribute
                *equally* to the meanoid profile unless these weights are
                specified.
 
-            By default, ``'gid_counts'``.
+            By default, :obj:`SupplyCurveField.GID_COUNTS`.
         n_profiles : int, optional
             Number of representative profiles to save to the output
             file. By default, ``1``.
         aggregate_profiles : bool, optional
             Flag to calculate the aggregate (weighted meanoid) profile
             for each supply curve point. This behavior is in lieu of
             finding the single profile per region closest to the
             meanoid. If you set this flag to ``True``, the `rep_method`,
             `err_method`, and `n_profiles` inputs will be forcibly set
             to the default values. By default, ``False``.
         """
 
         log_versions(logger)
-        logger.info('Finding representative profiles that are most similar '
-                    'to the weighted meanoid for each supply curve region.')
+        logger.info(
+            "Finding representative profiles that are most similar "
+            "to the weighted meanoid for each supply curve region."
+        )
 
         if reg_cols is None:
-            e = ('Need to define "reg_cols"! If you want a profile for each '
-                 'supply curve point, try setting "reg_cols" to a primary '
-                 'key such as "sc_gid".')
+            e = (
+                'Need to define "reg_cols"! If you want a profile for each '
+                'supply curve point, try setting "reg_cols" to a primary '
+                'key such as "sc_gid".'
+            )
             logger.error(e)
             raise ValueError(e)
-        elif isinstance(reg_cols, str):
+        if isinstance(reg_cols, str):
             reg_cols = [reg_cols]
         elif not isinstance(reg_cols, list):
             reg_cols = list(reg_cols)
 
         self._aggregate_profiles = aggregate_profiles
         if self._aggregate_profiles:
-            logger.info("Aggregate profiles input set to `True`. Setting "
-                        "'rep_method' to `'meanoid'`, 'err_method' to `None`, "
-                        "and 'n_profiles' to `1`")
-            rep_method = 'meanoid'
+            logger.info(
+                "Aggregate profiles input set to `True`. Setting "
+                "'rep_method' to `'meanoid'`, 'err_method' to `None`, "
+                "and 'n_profiles' to `1`"
+            )
+            rep_method = "meanoid"
             err_method = None
             n_profiles = 1
 
-        super().__init__(gen_fpath, rev_summary, reg_cols=reg_cols,
-                         cf_dset=cf_dset,
-                         rep_method=rep_method, err_method=err_method,
-                         weight=weight, n_profiles=n_profiles)
+        super().__init__(
+            gen_fpath,
+            rev_summary,
+            reg_cols=reg_cols,
+            cf_dset=cf_dset,
+            rep_method=rep_method,
+            err_method=err_method,
+            weight=weight,
+            n_profiles=n_profiles,
+        )
 
         self._set_meta()
         self._init_profiles()
 
     def _set_meta(self):
         """Set the rep profile meta data with each row being a unique
         combination of the region columns."""
         if self._err_method is None:
             self._meta = self._rev_summary
         else:
             self._meta = self._rev_summary.groupby(self._reg_cols)
             self._meta = (
-                self._meta['timezone']
+                self._meta[SupplyCurveField.TIMEZONE]
                 .apply(lambda x: stats.mode(x, keepdims=True).mode[0])
             )
             self._meta = self._meta.reset_index()
 
-        self._meta['rep_gen_gid'] = None
-        self._meta['rep_res_gid'] = None
+        self._meta["rep_gen_gid"] = None
+        self._meta["rep_res_gid"] = None
 
     def _get_mask(self, region_dict):
         """Get the mask for a given region and res class.
 
         Parameters
         ----------
         region_dict : dict
@@ -1050,137 +1131,170 @@
         -------
         mask : np.ndarray
             Boolean mask to filter rev_summary to the appropriate
             region_dict values.
         """
         mask = None
         for k, v in region_dict.items():
-            temp = (self._rev_summary[k] == v)
+            temp = self._rev_summary[k] == v
             if mask is None:
                 mask = temp
             else:
-                mask = (mask & temp)
+                mask = mask & temp
 
         return mask
 
     def _run_serial(self):
         """Compute all representative profiles in serial."""
 
-        logger.info('Running {} rep profile calculations in serial.'
-                    .format(len(self.meta)))
+        logger.info(
+            "Running {} rep profile calculations in serial.".format(
+                len(self.meta)
+            )
+        )
         meta_static = deepcopy(self.meta)
         for i, row in meta_static.iterrows():
-            region_dict = {k: v for (k, v) in row.to_dict().items()
-                           if k in self._reg_cols}
+            region_dict = {
+                k: v for (k, v) in row.to_dict().items() if k in self._reg_cols
+            }
             mask = self._get_mask(region_dict)
 
             if not any(mask):
-                logger.warning('Skipping profile {} out of {} '
-                               'for region: {} with no valid mask.'
-                               .format(i + 1, len(meta_static), region_dict))
+                logger.warning(
+                    "Skipping profile {} out of {} "
+                    "for region: {} with no valid mask.".format(
+                        i + 1, len(meta_static), region_dict
+                    )
+                )
             else:
-                logger.debug('Working on profile {} out of {} for region: {}'
-                             .format(i + 1, len(meta_static), region_dict))
+                logger.debug(
+                    "Working on profile {} out of {} for region: {}".format(
+                        i + 1, len(meta_static), region_dict
+                    )
+                )
                 out = RegionRepProfile.get_region_rep_profile(
-                    self._gen_fpath, self._rev_summary[mask],
-                    cf_dset=self._cf_dset, rep_method=self._rep_method,
-                    err_method=self._err_method, weight=self._weight,
-                    n_profiles=self._n_profiles)
+                    self._gen_fpath,
+                    self._rev_summary[mask],
+                    cf_dset=self._cf_dset,
+                    rep_method=self._rep_method,
+                    err_method=self._err_method,
+                    weight=self._weight,
+                    n_profiles=self._n_profiles,
+                )
                 profiles, _, ggids, rgids = out
-                logger.info('Profile {} out of {} complete '
-                            'for region: {}'
-                            .format(i + 1, len(meta_static), region_dict))
+                logger.info(
+                    "Profile {} out of {} complete " "for region: {}".format(
+                        i + 1, len(meta_static), region_dict
+                    )
+                )
 
                 for n in range(profiles.shape[1]):
                     self._profiles[n][:, i] = profiles[:, n]
 
                     if ggids is None:
-                        self._meta.at[i, 'rep_gen_gid'] = None
-                        self._meta.at[i, 'rep_res_gid'] = None
+                        self._meta.at[i, "rep_gen_gid"] = None
+                        self._meta.at[i, "rep_res_gid"] = None
                     elif len(ggids) == 1:
-                        self._meta.at[i, 'rep_gen_gid'] = ggids[0]
-                        self._meta.at[i, 'rep_res_gid'] = rgids[0]
+                        self._meta.at[i, "rep_gen_gid"] = ggids[0]
+                        self._meta.at[i, "rep_res_gid"] = rgids[0]
                     else:
-                        self._meta.at[i, 'rep_gen_gid'] = str(ggids)
-                        self._meta.at[i, 'rep_res_gid'] = str(rgids)
+                        self._meta.at[i, "rep_gen_gid"] = str(ggids)
+                        self._meta.at[i, "rep_res_gid"] = str(rgids)
 
     def _run_parallel(self, max_workers=None, pool_size=72):
         """Compute all representative profiles in parallel.
 
         Parameters
         ----------
         max_workers : int | None
             Number of parallel workers. 1 will run serial, None will use all
             available.
         pool_size : int
             Number of futures to submit to a single process pool for
             parallel futures.
         """
 
-        logger.info('Kicking off {} rep profile futures.'
-                    .format(len(self.meta)))
-
-        iter_chunks = np.array_split(self.meta.index.values,
-                                     np.ceil(len(self.meta) / pool_size))
+        logger.info(
+            "Kicking off {} rep profile futures.".format(len(self.meta))
+        )
+
+        iter_chunks = np.array_split(
+            self.meta.index.values, np.ceil(len(self.meta) / pool_size)
+        )
         n_complete = 0
         for iter_chunk in iter_chunks:
-            logger.debug('Starting process pool...')
+            logger.debug("Starting process pool...")
             futures = {}
-            loggers = [__name__, 'reV']
-            with SpawnProcessPool(max_workers=max_workers,
-                                  loggers=loggers) as exe:
+            loggers = [__name__, "reV"]
+            with SpawnProcessPool(
+                max_workers=max_workers, loggers=loggers
+            ) as exe:
                 for i in iter_chunk:
                     row = self.meta.loc[i, :]
-                    region_dict = {k: v for (k, v) in row.to_dict().items()
-                                   if k in self._reg_cols}
+                    region_dict = {
+                        k: v
+                        for (k, v) in row.to_dict().items()
+                        if k in self._reg_cols
+                    }
 
                     mask = self._get_mask(region_dict)
 
                     if not any(mask):
-                        logger.info('Skipping profile {} out of {} '
-                                    'for region: {} with no valid mask.'
-                                    .format(i + 1, len(self.meta),
-                                            region_dict))
+                        logger.info(
+                            "Skipping profile {} out of {} "
+                            "for region: {} with no valid mask.".format(
+                                i + 1, len(self.meta), region_dict
+                            )
+                        )
                     else:
                         future = exe.submit(
                             RegionRepProfile.get_region_rep_profile,
-                            self._gen_fpath, self._rev_summary[mask],
+                            self._gen_fpath,
+                            self._rev_summary[mask],
                             cf_dset=self._cf_dset,
                             rep_method=self._rep_method,
                             err_method=self._err_method,
                             weight=self._weight,
-                            n_profiles=self._n_profiles)
+                            n_profiles=self._n_profiles,
+                        )
 
                         futures[future] = [i, region_dict]
 
                 for future in as_completed(futures):
                     i, region_dict = futures[future]
                     profiles, _, ggids, rgids = future.result()
                     n_complete += 1
-                    logger.info('Future {} out of {} complete '
-                                'for region: {}'
-                                .format(n_complete, len(self.meta),
-                                        region_dict))
-                    log_mem(logger, log_level='DEBUG')
+                    logger.info(
+                        "Future {} out of {} complete "
+                        "for region: {}".format(
+                            n_complete, len(self.meta), region_dict
+                        )
+                    )
+                    log_mem(logger, log_level="DEBUG")
 
                     for n in range(profiles.shape[1]):
                         self._profiles[n][:, i] = profiles[:, n]
 
                     if ggids is None:
-                        self._meta.at[i, 'rep_gen_gid'] = None
-                        self._meta.at[i, 'rep_res_gid'] = None
+                        self._meta.at[i, "rep_gen_gid"] = None
+                        self._meta.at[i, "rep_res_gid"] = None
                     elif len(ggids) == 1:
-                        self._meta.at[i, 'rep_gen_gid'] = ggids[0]
-                        self._meta.at[i, 'rep_res_gid'] = rgids[0]
+                        self._meta.at[i, "rep_gen_gid"] = ggids[0]
+                        self._meta.at[i, "rep_res_gid"] = rgids[0]
                     else:
-                        self._meta.at[i, 'rep_gen_gid'] = str(ggids)
-                        self._meta.at[i, 'rep_res_gid'] = str(rgids)
+                        self._meta.at[i, "rep_gen_gid"] = str(ggids)
+                        self._meta.at[i, "rep_res_gid"] = str(rgids)
 
-    def run(self, fout=None, save_rev_summary=True, scaled_precision=False,
-            max_workers=None):
+    def run(
+        self,
+        fout=None,
+        save_rev_summary=True,
+        scaled_precision=False,
+        max_workers=None,
+    ):
         """
         Run representative profiles in serial or parallel and save to disc
 
         Parameters
         ----------
         fout : str, optional
             Filepath to output HDF5 file. If ``None``, output data are
@@ -1200,16 +1314,21 @@
         if max_workers == 1:
             self._run_serial()
         else:
             self._run_parallel(max_workers=max_workers)
 
         if fout is not None:
             if self._aggregate_profiles:
-                logger.info("Aggregate profiles input set to `True`. Setting "
-                            "'save_rev_summary' input to `False`")
+                logger.info(
+                    "Aggregate profiles input set to `True`. Setting "
+                    "'save_rev_summary' input to `False`"
+                )
                 save_rev_summary = False
-            self.save_profiles(fout, save_rev_summary=save_rev_summary,
-                               scaled_precision=scaled_precision)
+            self.save_profiles(
+                fout,
+                save_rev_summary=save_rev_summary,
+                scaled_precision=scaled_precision,
+            )
 
-        logger.info('Representative profiles complete!')
+        logger.info("Representative profiles complete!")
 
         return fout
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/aggregation.py` & `NREL-reV-0.8.9/reV/supply_curve/aggregation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 # -*- coding: utf-8 -*-
-"""
-reV aggregation framework.
-"""
+"""reV aggregation framework."""
+
+import logging
+import os
 from abc import ABC, abstractmethod
+
 import h5py
-import logging
 import numpy as np
-import os
 import pandas as pd
+from rex.resource import Resource
+from rex.utilities.execution import SpawnProcessPool
+from rex.utilities.loggers import log_mem
 
-from reV.handlers.outputs import Outputs
 from reV.handlers.exclusions import ExclusionLayers
+from reV.handlers.outputs import Outputs
 from reV.supply_curve.exclusions import ExclusionMaskFromDict
 from reV.supply_curve.extent import SupplyCurveExtent
-from reV.supply_curve.tech_mapping import TechMapping
 from reV.supply_curve.points import AggregationSupplyCurvePoint
-from reV.utilities.exceptions import (EmptySupplyCurvePointError,
-                                      FileInputError, SupplyCurveInputError)
-from reV.utilities import log_versions
-
-from rex.resource import Resource
-from rex.utilities.execution import SpawnProcessPool
-from rex.utilities.loggers import log_mem
+from reV.supply_curve.tech_mapping import TechMapping
+from reV.utilities import ResourceMetaField, SupplyCurveField, log_versions
+from reV.utilities.exceptions import (
+    EmptySupplyCurvePointError,
+    FileInputError,
+    SupplyCurveInputError,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractAggFileHandler(ABC):
     """Simple framework to handle aggregation file context managers."""
 
-    def __init__(self, excl_fpath, excl_dict=None, area_filter_kernel='queen',
-                 min_area=None):
+    def __init__(
+        self,
+        excl_fpath,
+        excl_dict=None,
+        area_filter_kernel="queen",
+        min_area=None,
+    ):
         """
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
             (can be one or more filepaths).
         excl_dict : dict | None
@@ -47,17 +54,20 @@
             Contiguous area filter method to use on final exclusions mask,
             by default 'queen'
         min_area : float, optional
             Minimum required contiguous area filter in sq-km,
             by default None
         """
         self._excl_fpath = excl_fpath
-        self._excl = ExclusionMaskFromDict(excl_fpath, layers_dict=excl_dict,
-                                           min_area=min_area,
-                                           kernel=area_filter_kernel)
+        self._excl = ExclusionMaskFromDict(
+            excl_fpath,
+            layers_dict=excl_dict,
+            min_area=min_area,
+            kernel=area_filter_kernel,
+        )
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.close()
         if type is not None:
@@ -91,17 +101,23 @@
     Framework to handle aggregation file context manager:
     - exclusions .h5 file
     - h5 file to be aggregated
     """
 
     DEFAULT_H5_HANDLER = Resource
 
-    def __init__(self, excl_fpath, h5_fpath, excl_dict=None,
-                 area_filter_kernel='queen', min_area=None,
-                 h5_handler=None):
+    def __init__(
+        self,
+        excl_fpath,
+        h5_fpath,
+        excl_dict=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        h5_handler=None,
+    ):
         """
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
             (can be one or more filepaths).
         h5_fpath : str
@@ -117,17 +133,20 @@
             by default 'queen'
         min_area : float, optional
             Minimum required contiguous area filter in sq-km, by default None
         h5_handler : rex.Resource | None
             Optional special handler similar to the rex.Resource handler which
             is default.
         """
-        super().__init__(excl_fpath, excl_dict=excl_dict,
-                         area_filter_kernel=area_filter_kernel,
-                         min_area=min_area)
+        super().__init__(
+            excl_fpath,
+            excl_dict=excl_dict,
+            area_filter_kernel=area_filter_kernel,
+            min_area=min_area,
+        )
 
         if h5_handler is None:
             self._h5 = Resource(h5_fpath)
         else:
             self._h5 = h5_handler(h5_fpath)
 
     @property
@@ -148,18 +167,27 @@
         self._h5.close()
 
 
 class BaseAggregation(ABC):
     """Abstract supply curve points aggregation framework based on only an
     exclusion file and techmap."""
 
-    def __init__(self, excl_fpath, tm_dset, excl_dict=None,
-                 area_filter_kernel='queen', min_area=None,
-                 resolution=64, excl_area=None, res_fpath=None, gids=None,
-                 pre_extract_inclusions=False):
+    def __init__(
+        self,
+        excl_fpath,
+        tm_dset,
+        excl_dict=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        resolution=64,
+        excl_area=None,
+        res_fpath=None,
+        gids=None,
+        pre_extract_inclusions=False,
+    ):
         """
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
             (can be one or more filepaths).
         tm_dset : str
@@ -204,63 +232,75 @@
         self._pre_extract_inclusions = pre_extract_inclusions
         self._excl_area = self._get_excl_area(excl_fpath, excl_area=excl_area)
         self._shape = None
 
         self._validate_tech_mapping()
 
         if pre_extract_inclusions:
-            self._inclusion_mask = \
+            self._inclusion_mask = (
                 ExclusionMaskFromDict.extract_inclusion_mask(
-                    excl_fpath, tm_dset,
+                    excl_fpath,
+                    tm_dset,
                     excl_dict=excl_dict,
                     area_filter_kernel=area_filter_kernel,
-                    min_area=min_area)
+                    min_area=min_area,
+                )
+            )
         else:
             self._inclusion_mask = None
 
     def _validate_tech_mapping(self):
         """Check that tech mapping exists and create it if it doesn't"""
 
         with ExclusionLayers(self._excl_fpath) as f:
             dsets = f.h5.dsets
 
         excl_fp_is_str = isinstance(self._excl_fpath, str)
         tm_in_excl = self._tm_dset in dsets
         if tm_in_excl:
             logger.info('Found techmap "{}".'.format(self._tm_dset))
         elif not tm_in_excl and not excl_fp_is_str:
-            msg = ('Could not find techmap dataset "{}" and cannot run '
-                   'techmap with arbitrary multiple exclusion filepaths '
-                   'to write to: {}'.format(self._tm_dset, self._excl_fpath))
+            msg = (
+                'Could not find techmap dataset "{}" and cannot run '
+                "techmap with arbitrary multiple exclusion filepaths "
+                "to write to: {}".format(self._tm_dset, self._excl_fpath)
+            )
             logger.error(msg)
             raise RuntimeError(msg)
         else:
-            logger.info('Could not find techmap "{}". Running techmap module.'
-                        .format(self._tm_dset))
+            logger.info(
+                'Could not find techmap "{}". Running techmap module.'.format(
+                    self._tm_dset
+                )
+            )
             try:
-                TechMapping.run(self._excl_fpath, self._res_fpath,
-                                dset=self._tm_dset)
+                TechMapping.run(
+                    self._excl_fpath, self._res_fpath, dset=self._tm_dset
+                )
             except Exception as e:
-                msg = ('TechMapping process failed. Received the '
-                       'following error:\n{}'.format(e))
+                msg = (
+                    "TechMapping process failed. Received the "
+                    "following error:\n{}".format(e)
+                )
                 logger.exception(msg)
                 raise RuntimeError(msg) from e
 
     @property
     def gids(self):
         """
         1D array of supply curve point gids to aggregate
 
         Returns
         -------
         ndarray
         """
         if self._gids is None:
-            with SupplyCurveExtent(self._excl_fpath,
-                                   resolution=self._resolution) as sc:
+            with SupplyCurveExtent(
+                self._excl_fpath, resolution=self._resolution
+            ) as sc:
                 self._gids = sc.valid_sc_points(self._tm_dset)
         elif np.issubdtype(type(self._gids), np.number):
             self._gids = np.array([self._gids])
         elif not isinstance(self._gids, np.ndarray):
             self._gids = np.array(self._gids)
 
         return self._gids
@@ -270,16 +310,17 @@
         """Get the shape of the full exclusions raster.
 
         Returns
         -------
         tuple
         """
         if self._shape is None:
-            with SupplyCurveExtent(self._excl_fpath,
-                                   resolution=self._resolution) as sc:
+            with SupplyCurveExtent(
+                self._excl_fpath, resolution=self._resolution
+            ) as sc:
                 self._shape = sc.exclusions.shape
 
         return self._shape
 
     @staticmethod
     def _get_excl_area(excl_fpath, excl_area=None):
         """
@@ -297,22 +338,26 @@
 
         Returns
         -------
         excl_area : float
             Area of an exclusion pixel in km2
         """
         if excl_area is None:
-            logger.debug('Setting the exclusion area from the area of a pixel '
-                         'in {}'.format(excl_fpath))
+            logger.debug(
+                "Setting the exclusion area from the area of a pixel "
+                "in {}".format(excl_fpath)
+            )
             with ExclusionLayers(excl_fpath) as excl:
                 excl_area = excl.pixel_area
 
         if excl_area is None:
-            e = ('No exclusion pixel area was input and could not parse '
-                 'area from the exclusion file attributes!')
+            e = (
+                "No exclusion pixel area was input and could not parse "
+                "area from the exclusion file attributes!"
+            )
             logger.error(e)
             raise SupplyCurveInputError(e)
 
         return excl_area
 
     @staticmethod
     def _check_inclusion_mask(inclusion_mask, gids, excl_shape):
@@ -333,22 +378,25 @@
             Full exclusion layers shape
         """
         if isinstance(inclusion_mask, dict):
             assert len(inclusion_mask) == len(gids)
         elif isinstance(inclusion_mask, np.ndarray):
             assert inclusion_mask.shape == excl_shape
         elif inclusion_mask is not None:
-            msg = ('Expected inclusion_mask to be dict or array but received '
-                   '{}'.format(type(inclusion_mask)))
+            msg = (
+                "Expected inclusion_mask to be dict or array but received "
+                "{}".format(type(inclusion_mask))
+            )
             logger.error(msg)
             raise SupplyCurveInputError(msg)
 
     @staticmethod
-    def _get_gid_inclusion_mask(inclusion_mask, gid, slice_lookup,
-                                resolution=64):
+    def _get_gid_inclusion_mask(
+        inclusion_mask, gid, slice_lookup, resolution=64
+    ):
         """
         Get inclusion mask for desired gid
 
         Parameters
         ----------
         inclusion_mask : np.ndarray | dict | optional
             2D array pre-extracted inclusion mask where 1 is included and 0 is
@@ -377,16 +425,18 @@
             gid_inclusions = inclusion_mask[gid]
             assert gid_inclusions.shape[0] <= resolution
             assert gid_inclusions.shape[1] <= resolution
         elif isinstance(inclusion_mask, np.ndarray):
             row_slice, col_slice = slice_lookup[gid]
             gid_inclusions = inclusion_mask[row_slice, col_slice]
         elif inclusion_mask is not None:
-            msg = ('Expected inclusion_mask to be dict or array but received '
-                   '{}'.format(type(inclusion_mask)))
+            msg = (
+                "Expected inclusion_mask to be dict or array but received "
+                "{}".format(type(inclusion_mask))
+            )
             logger.error(msg)
             raise SupplyCurveInputError(msg)
 
         return gid_inclusions
 
     @staticmethod
     def _parse_gen_index(gen_fpath):
@@ -403,50 +453,67 @@
         -------
         gen_index : np.ndarray
             Array of generation gids with array index equal to resource gid.
             Array value is -1 if the resource index was not used in the
             generation run.
         """
 
-        if gen_fpath.endswith('.h5'):
+        if gen_fpath.endswith(".h5"):
             with Resource(gen_fpath) as f:
                 gen_index = f.meta
-        elif gen_fpath.endswith('.csv'):
+        elif gen_fpath.endswith(".csv"):
             gen_index = pd.read_csv(gen_fpath)
         else:
-            msg = ('Could not recognize gen_fpath input, needs to be reV gen '
-                   'output h5 or project points csv but received: {}'
-                   .format(gen_fpath))
+            msg = (
+                "Could not recognize gen_fpath input, needs to be reV gen "
+                "output h5 or project points csv but received: {}".format(
+                    gen_fpath
+                )
+            )
             logger.error(msg)
             raise FileInputError(msg)
 
-        if 'gid' in gen_index:
-            gen_index = gen_index.rename(columns={'gid': 'res_gids'})
-            gen_index['gen_gids'] = gen_index.index
-            gen_index = gen_index[['res_gids', 'gen_gids']]
-            gen_index = gen_index.set_index(keys='res_gids')
-            gen_index = \
-                gen_index.reindex(range(int(gen_index.index.max() + 1)))
-            gen_index = gen_index['gen_gids'].values
+        if ResourceMetaField.GID in gen_index:
+            gen_index = gen_index.rename(
+                columns={ResourceMetaField.GID: SupplyCurveField.RES_GIDS}
+            )
+            gen_index[SupplyCurveField.GEN_GIDS] = gen_index.index
+            gen_index = gen_index[
+                [SupplyCurveField.RES_GIDS, SupplyCurveField.GEN_GIDS]
+            ]
+            gen_index = gen_index.set_index(keys=SupplyCurveField.RES_GIDS)
+            gen_index = gen_index.reindex(
+                range(int(gen_index.index.max() + 1))
+            )
+            gen_index = gen_index[SupplyCurveField.GEN_GIDS].values
             gen_index[np.isnan(gen_index)] = -1
             gen_index = gen_index.astype(np.int32)
         else:
             gen_index = None
 
         return gen_index
 
 
 class Aggregation(BaseAggregation):
     """Concrete but generalized aggregation framework to aggregate ANY reV h5
     file to a supply curve grid (based on an aggregated exclusion grid)."""
 
-    def __init__(self, excl_fpath, tm_dset, *agg_dset,
-                 excl_dict=None, area_filter_kernel='queen', min_area=None,
-                 resolution=64, excl_area=None, gids=None,
-                 pre_extract_inclusions=False):
+    def __init__(
+        self,
+        excl_fpath,
+        tm_dset,
+        *agg_dset,
+        excl_dict=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        resolution=64,
+        excl_area=None,
+        gids=None,
+        pre_extract_inclusions=False,
+    ):
         """
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
             (can be one or more filepaths).
         tm_dset : str
@@ -482,60 +549,84 @@
             extent, by default None
         pre_extract_inclusions : bool, optional
             Optional flag to pre-extract/compute the inclusion mask from the
             provided excl_dict, by default False. Typically faster to compute
             the inclusion mask on the fly with parallel workers.
         """
         log_versions(logger)
-        logger.info('Initializing Aggregation...')
-        logger.debug('Exclusion filepath: {}'.format(excl_fpath))
-        logger.debug('Exclusion dict: {}'.format(excl_dict))
-
-        super().__init__(excl_fpath, tm_dset, excl_dict=excl_dict,
-                         area_filter_kernel=area_filter_kernel,
-                         min_area=min_area, resolution=resolution,
-                         excl_area=excl_area, gids=gids,
-                         pre_extract_inclusions=pre_extract_inclusions)
+        logger.info("Initializing Aggregation...")
+        logger.debug("Exclusion filepath: {}".format(excl_fpath))
+        logger.debug("Exclusion dict: {}".format(excl_dict))
+
+        super().__init__(
+            excl_fpath,
+            tm_dset,
+            excl_dict=excl_dict,
+            area_filter_kernel=area_filter_kernel,
+            min_area=min_area,
+            resolution=resolution,
+            excl_area=excl_area,
+            gids=gids,
+            pre_extract_inclusions=pre_extract_inclusions,
+        )
 
         if isinstance(agg_dset, str):
-            agg_dset = (agg_dset, )
+            agg_dset = (agg_dset,)
 
         self._agg_dsets = agg_dset
 
     def _check_files(self, h5_fpath):
         """Do a preflight check on input files"""
 
         if not os.path.exists(self._excl_fpath):
-            raise FileNotFoundError('Could not find required exclusions file: '
-                                    '{}'.format(self._excl_fpath))
+            raise FileNotFoundError(
+                "Could not find required exclusions file: " "{}".format(
+                    self._excl_fpath
+                )
+            )
 
         if not os.path.exists(h5_fpath):
-            raise FileNotFoundError('Could not find required h5 file: '
-                                    '{}'.format(h5_fpath))
+            raise FileNotFoundError(
+                "Could not find required h5 file: " "{}".format(h5_fpath)
+            )
 
-        with h5py.File(self._excl_fpath, 'r') as f:
+        with h5py.File(self._excl_fpath, "r") as f:
             if self._tm_dset not in f:
-                raise FileInputError('Could not find techmap dataset "{}" '
-                                     'in exclusions file: {}'
-                                     .format(self._tm_dset,
-                                             self._excl_fpath))
+                raise FileInputError(
+                    'Could not find techmap dataset "{}" '
+                    "in exclusions file: {}".format(
+                        self._tm_dset, self._excl_fpath
+                    )
+                )
 
         with Resource(h5_fpath) as f:
             for dset in self._agg_dsets:
                 if dset not in f:
-                    raise FileInputError('Could not find provided dataset "{}"'
-                                         ' in h5 file: {}'
-                                         .format(dset, h5_fpath))
+                    raise FileInputError(
+                        'Could not find provided dataset "{}"'
+                        " in h5 file: {}".format(dset, h5_fpath)
+                    )
 
     @classmethod
-    def run_serial(cls, excl_fpath, h5_fpath, tm_dset, *agg_dset,
-                   agg_method='mean', excl_dict=None, inclusion_mask=None,
-                   area_filter_kernel='queen', min_area=None,
-                   resolution=64, excl_area=0.0081, gids=None,
-                   gen_index=None):
+    def run_serial(
+        cls,
+        excl_fpath,
+        h5_fpath,
+        tm_dset,
+        *agg_dset,
+        agg_method="mean",
+        excl_dict=None,
+        inclusion_mask=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        resolution=64,
+        excl_area=0.0081,
+        gids=None,
+        gen_index=None,
+    ):
         """
         Standalone method to aggregate - can be parallelized.
 
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
@@ -598,61 +689,78 @@
                 gids = [gids]
 
             slice_lookup = sc.get_slice_lookup(gids)
 
         cls._check_inclusion_mask(inclusion_mask, gids, exclusion_shape)
 
         # pre-extract handlers so they are not repeatedly initialized
-        file_kwargs = {'excl_dict': excl_dict,
-                       'area_filter_kernel': area_filter_kernel,
-                       'min_area': min_area}
-        dsets = agg_dset + ('meta', )
+        file_kwargs = {
+            "excl_dict": excl_dict,
+            "area_filter_kernel": area_filter_kernel,
+            "min_area": min_area,
+        }
+        dsets = (
+            *agg_dset,
+            "meta",
+        )
         agg_out = {ds: [] for ds in dsets}
         with AggFileHandler(excl_fpath, h5_fpath, **file_kwargs) as fh:
             n_finished = 0
             for gid in gids:
                 gid_inclusions = cls._get_gid_inclusion_mask(
-                    inclusion_mask, gid, slice_lookup,
-                    resolution=resolution)
+                    inclusion_mask, gid, slice_lookup, resolution=resolution
+                )
                 try:
                     gid_out = AggregationSupplyCurvePoint.run(
                         gid,
                         fh.exclusions,
                         fh.h5,
                         tm_dset,
                         *agg_dset,
                         agg_method=agg_method,
                         excl_dict=excl_dict,
                         inclusion_mask=gid_inclusions,
                         resolution=resolution,
                         excl_area=excl_area,
                         exclusion_shape=exclusion_shape,
                         close=False,
-                        gen_index=gen_index)
+                        gen_index=gen_index,
+                    )
 
                 except EmptySupplyCurvePointError:
-                    logger.debug('SC gid {} is fully excluded or does not '
-                                 'have any valid source data!'.format(gid))
+                    logger.debug(
+                        "SC gid {} is fully excluded or does not "
+                        "have any valid source data!".format(gid)
+                    )
                 except Exception as e:
-                    msg = 'SC gid {} failed!'.format(gid)
+                    msg = "SC gid {} failed!".format(gid)
                     logger.exception(msg)
                     raise RuntimeError(msg) from e
                 else:
                     n_finished += 1
-                    logger.debug('Serial aggregation: '
-                                 '{} out of {} points complete'
-                                 .format(n_finished, len(gids)))
+                    logger.debug(
+                        "Serial aggregation: "
+                        "{} out of {} points complete".format(
+                            n_finished, len(gids)
+                        )
+                    )
                     log_mem(logger)
                     for k, v in gid_out.items():
                         agg_out[k].append(v)
 
         return agg_out
 
-    def run_parallel(self, h5_fpath, agg_method='mean', excl_area=None,
-                     max_workers=None, sites_per_worker=100):
+    def run_parallel(
+        self,
+        h5_fpath,
+        agg_method="mean",
+        excl_area=None,
+        max_workers=None,
+        sites_per_worker=100,
+    ):
         """
         Aggregate in parallel
 
         Parameters
         ----------
         h5_fpath : str
             Filepath to .h5 file to aggregate
@@ -677,72 +785,88 @@
         gen_index = self._parse_gen_index(h5_fpath)
 
         slice_lookup = None
         chunks = int(np.ceil(len(self.gids) / sites_per_worker))
         chunks = np.array_split(self.gids, chunks)
 
         if self._inclusion_mask is not None:
-            with SupplyCurveExtent(self._excl_fpath,
-                                   resolution=self._resolution) as sc:
+            with SupplyCurveExtent(
+                self._excl_fpath, resolution=self._resolution
+            ) as sc:
                 assert sc.exclusions.shape == self._inclusion_mask.shape
                 slice_lookup = sc.get_slice_lookup(self.gids)
 
-        logger.info('Running supply curve point aggregation for '
-                    'points {} through {} at a resolution of {} '
-                    'on {} cores in {} chunks.'
-                    .format(self.gids[0], self.gids[-1], self._resolution,
-                            max_workers, len(chunks)))
+        logger.info(
+            "Running supply curve point aggregation for "
+            "points {} through {} at a resolution of {} "
+            "on {} cores in {} chunks.".format(
+                self.gids[0],
+                self.gids[-1],
+                self._resolution,
+                max_workers,
+                len(chunks),
+            )
+        )
 
         n_finished = 0
         futures = []
-        dsets = self._agg_dsets + ('meta', )
+        dsets = self._agg_dsets + ("meta",)
         agg_out = {ds: [] for ds in dsets}
-        loggers = [__name__, 'reV.supply_curve.points', 'reV']
+        loggers = [__name__, "reV.supply_curve.points", "reV"]
         with SpawnProcessPool(max_workers=max_workers, loggers=loggers) as exe:
             # iterate through split executions, submitting each to worker
             for gid_set in chunks:
                 # submit executions and append to futures list
                 chunk_incl_masks = None
                 if self._inclusion_mask is not None:
                     chunk_incl_masks = {}
                     for gid in gid_set:
                         rs, cs = slice_lookup[gid]
                         chunk_incl_masks[gid] = self._inclusion_mask[rs, cs]
 
                 # submit executions and append to futures list
-                futures.append(exe.submit(
-                    self.run_serial,
-                    self._excl_fpath,
-                    h5_fpath,
-                    self._tm_dset,
-                    *self._agg_dsets,
-                    agg_method=agg_method,
-                    excl_dict=self._excl_dict,
-                    inclusion_mask=chunk_incl_masks,
-                    area_filter_kernel=self._area_filter_kernel,
-                    min_area=self._min_area,
-                    resolution=self._resolution,
-                    excl_area=excl_area,
-                    gids=gid_set,
-                    gen_index=gen_index))
+                futures.append(
+                    exe.submit(
+                        self.run_serial,
+                        self._excl_fpath,
+                        h5_fpath,
+                        self._tm_dset,
+                        *self._agg_dsets,
+                        agg_method=agg_method,
+                        excl_dict=self._excl_dict,
+                        inclusion_mask=chunk_incl_masks,
+                        area_filter_kernel=self._area_filter_kernel,
+                        min_area=self._min_area,
+                        resolution=self._resolution,
+                        excl_area=excl_area,
+                        gids=gid_set,
+                        gen_index=gen_index,
+                    )
+                )
 
             # gather results
             for future in futures:
                 n_finished += 1
-                logger.info('Parallel aggregation futures collected: '
-                            '{} out of {}'
-                            .format(n_finished, len(chunks)))
+                logger.info(
+                    "Parallel aggregation futures collected: "
+                    "{} out of {}".format(n_finished, len(chunks))
+                )
                 for k, v in future.result().items():
                     if v:
                         agg_out[k].extend(v)
 
         return agg_out
 
-    def aggregate(self, h5_fpath, agg_method='mean', max_workers=None,
-                  sites_per_worker=100):
+    def aggregate(
+        self,
+        h5_fpath,
+        agg_method="mean",
+        max_workers=None,
+        sites_per_worker=100,
+    ):
         """
         Aggregate with given agg_method
 
         Parameters
         ----------
         h5_fpath : str
             Filepath to .h5 file to aggregate
@@ -762,46 +886,52 @@
         """
         if max_workers is None:
             max_workers = os.cpu_count()
 
         if max_workers == 1:
             self._check_files(h5_fpath)
             gen_index = self._parse_gen_index(h5_fpath)
-            agg = self.run_serial(self._excl_fpath,
-                                  h5_fpath,
-                                  self._tm_dset,
-                                  *self._agg_dsets,
-                                  agg_method=agg_method,
-                                  excl_dict=self._excl_dict,
-                                  gids=self.gids,
-                                  inclusion_mask=self._inclusion_mask,
-                                  area_filter_kernel=self._area_filter_kernel,
-                                  min_area=self._min_area,
-                                  resolution=self._resolution,
-                                  excl_area=self._excl_area,
-                                  gen_index=gen_index)
+            agg = self.run_serial(
+                self._excl_fpath,
+                h5_fpath,
+                self._tm_dset,
+                *self._agg_dsets,
+                agg_method=agg_method,
+                excl_dict=self._excl_dict,
+                gids=self.gids,
+                inclusion_mask=self._inclusion_mask,
+                area_filter_kernel=self._area_filter_kernel,
+                min_area=self._min_area,
+                resolution=self._resolution,
+                excl_area=self._excl_area,
+                gen_index=gen_index,
+            )
         else:
-            agg = self.run_parallel(h5_fpath=h5_fpath,
-                                    agg_method=agg_method,
-                                    excl_area=self._excl_area,
-                                    max_workers=max_workers,
-                                    sites_per_worker=sites_per_worker)
-
-        if not agg['meta']:
-            e = ('Supply curve aggregation found no non-excluded SC points. '
-                 'Please check your exclusions or subset SC GID selection.')
+            agg = self.run_parallel(
+                h5_fpath=h5_fpath,
+                agg_method=agg_method,
+                excl_area=self._excl_area,
+                max_workers=max_workers,
+                sites_per_worker=sites_per_worker,
+            )
+
+        if not agg["meta"]:
+            e = (
+                "Supply curve aggregation found no non-excluded SC points. "
+                "Please check your exclusions or subset SC GID selection."
+            )
             logger.error(e)
             raise EmptySupplyCurvePointError(e)
 
         for k, v in agg.items():
-            if k == 'meta':
+            if k == "meta":
                 v = pd.concat(v, axis=1).T
-                v = v.sort_values('sc_point_gid')
+                v = v.sort_values(SupplyCurveField.SC_POINT_GID)
                 v = v.reset_index(drop=True)
-                v.index.name = 'sc_gid'
+                v.index.name = SupplyCurveField.SC_GID
                 agg[k] = v
             else:
                 v = np.dstack(v)[0]
                 if v.shape[0] == 1:
                     v = v.flatten()
 
                 agg[k] = v
@@ -817,15 +947,15 @@
         ----------
         out_fpath : str
             Output .h5 file path
         aggregation : dict
             Aggregated values for each aggregation dataset
         """
         agg_out = aggregation.copy()
-        meta = agg_out.pop('meta').reset_index()
+        meta = agg_out.pop("meta").reset_index()
         for c in meta.columns:
             try:
                 meta[c] = pd.to_numeric(meta[c])
             except (ValueError, TypeError):
                 pass
 
         dsets = []
@@ -836,36 +966,57 @@
         time_index = None
         with Resource(h5_fpath) as f:
             for dset, data in agg_out.items():
                 dsets.append(dset)
                 shape = data.shape
                 shapes[dset] = shape
                 if len(data.shape) == 2:
-                    if ('time_index' in f) and (shape[0] == f.shape[0]):
+                    if ("time_index" in f) and (shape[0] == f.shape[0]):
                         if time_index is None:
                             time_index = f.time_index
 
                 attrs[dset] = f.get_attrs(dset=dset)
                 _, dtype, chunk = f.get_dset_properties(dset)
                 chunks[dset] = chunk
                 dtypes[dset] = dtype
 
-        Outputs.init_h5(out_fpath, dsets, shapes, attrs, chunks, dtypes,
-                        meta, time_index=time_index)
+        Outputs.init_h5(
+            out_fpath,
+            dsets,
+            shapes,
+            attrs,
+            chunks,
+            dtypes,
+            meta,
+            time_index=time_index,
+        )
 
-        with Outputs(out_fpath, mode='a') as out:
+        with Outputs(out_fpath, mode="a") as out:
             for dset, data in agg_out.items():
                 out[dset] = data
 
     @classmethod
-    def run(cls, excl_fpath, h5_fpath, tm_dset, *agg_dset,
-            excl_dict=None, area_filter_kernel='queen', min_area=None,
-            resolution=64, excl_area=None, gids=None,
-            pre_extract_inclusions=False, agg_method='mean', max_workers=None,
-            sites_per_worker=100, out_fpath=None):
+    def run(
+        cls,
+        excl_fpath,
+        h5_fpath,
+        tm_dset,
+        *agg_dset,
+        excl_dict=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        resolution=64,
+        excl_area=None,
+        gids=None,
+        pre_extract_inclusions=False,
+        agg_method="mean",
+        max_workers=None,
+        sites_per_worker=100,
+        out_fpath=None,
+    ):
         """Get the supply curve points aggregation summary.
 
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
             (can be one or more filepaths).
@@ -919,21 +1070,31 @@
 
         Returns
         -------
         agg : dict
             Aggregated values for each aggregation dataset
         """
 
-        agg = cls(excl_fpath, tm_dset, *agg_dset,
-                  excl_dict=excl_dict, area_filter_kernel=area_filter_kernel,
-                  min_area=min_area, resolution=resolution,
-                  excl_area=excl_area, gids=gids,
-                  pre_extract_inclusions=pre_extract_inclusions)
-
-        aggregation = agg.aggregate(h5_fpath=h5_fpath, agg_method=agg_method,
-                                    max_workers=max_workers,
-                                    sites_per_worker=sites_per_worker)
+        agg = cls(
+            excl_fpath,
+            tm_dset,
+            *agg_dset,
+            excl_dict=excl_dict,
+            area_filter_kernel=area_filter_kernel,
+            min_area=min_area,
+            resolution=resolution,
+            excl_area=excl_area,
+            gids=gids,
+            pre_extract_inclusions=pre_extract_inclusions,
+        )
+
+        aggregation = agg.aggregate(
+            h5_fpath=h5_fpath,
+            agg_method=agg_method,
+            max_workers=max_workers,
+            sites_per_worker=sites_per_worker,
+        )
 
         if out_fpath is not None:
             agg.save_agg_to_h5(h5_fpath, out_fpath, aggregation)
 
         return aggregation
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/cli_sc_aggregation.py` & `NREL-reV-0.8.9/reV/supply_curve/cli_sc_aggregation.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/supply_curve/cli_supply_curve.py` & `NREL-reV-0.8.9/reV/supply_curve/cli_supply_curve.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/supply_curve/competitive_wind_farms.py` & `NREL-reV-0.8.9/reV/supply_curve/competitive_wind_farms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 Competitive Wind Farms exclusion handler
 """
 import logging
-import numpy as np
 
+import numpy as np
 from rex.utilities.utilities import parse_table
 
+from reV.utilities import SupplyCurveField
+
 logger = logging.getLogger(__name__)
 
 
 class CompetitiveWindFarms:
     """
     Handle competitive wind farm exclusion during supply curve sorting
     """
@@ -29,38 +31,44 @@
             Number of prominent directions to use, by default 2
         offshore : bool
             Flag as to whether offshore farms should be included during
             CompetitiveWindFarms
         """
         self._wind_dirs = self._parse_wind_dirs(wind_dirs)
 
-        self._sc_gids, self._sc_point_gids, self._mask = \
-            self._parse_sc_points(sc_points, offshore=offshore)
+        self._sc_gids, self._sc_point_gids, self._mask = self._parse_sc_points(
+            sc_points, offshore=offshore
+        )
 
         self._offshore = offshore
 
         valid = np.isin(self.sc_point_gids, self._wind_dirs.index)
         if not np.all(valid):
-            msg = ("'sc_points contains sc_point_gid values that do not "
-                   "correspond to valid 'wind_dirs' sc_point_gids:\n{}"
-                   .format(self.sc_point_gids[~valid]))
+            msg = (
+                "'sc_points contains sc_point_gid values that do not "
+                "correspond to valid 'wind_dirs' sc_point_gids:\n{}".format(
+                    self.sc_point_gids[~valid]
+                )
+            )
             logger.error(msg)
             raise RuntimeError(msg)
 
         mask = self._wind_dirs.index.isin(self._sc_point_gids.keys())
         self._wind_dirs = self._wind_dirs.loc[mask]
-        self._upwind, self._downwind = self._get_neighbors(self._wind_dirs,
-                                                           n_dirs=n_dirs)
+        self._upwind, self._downwind = self._get_neighbors(
+            self._wind_dirs, n_dirs=n_dirs
+        )
 
     def __repr__(self):
         gids = len(self._upwind)
         # pylint: disable=unsubscriptable-object
         neighbors = len(self._upwind.values[0])
-        msg = ("{} with {} sc_point_gids and {} prominent directions"
-               .format(self.__class__.__name__, gids, neighbors))
+        msg = "{} with {} sc_point_gids and {} prominent directions".format(
+            self.__class__.__name__, gids, neighbors
+        )
 
         return msg
 
     def __getitem__(self, keys):
         """
         Map gid for given mapping
 
@@ -72,31 +80,33 @@
         Returns
         -------
         gid(s) : int | list
             Mapped gid(s) for given mapping
         """
         if not isinstance(keys, tuple):
             msg = ("{} must be a tuple of form (source, gid) where source is: "
-                   "'sc_gid', 'sc_point_gid',  or 'upwind', 'downwind'"
-                   .format(keys))
+                   "{}, '{}',  or 'upwind', 'downwind'"
+                   .format(keys, SupplyCurveField.SC_GID,
+                           SupplyCurveField.SC_POINT_GID))
             logger.error(msg)
             raise ValueError(msg)
 
         source, gid = keys
-        if source == 'sc_point_gid':
+        if source == SupplyCurveField.SC_POINT_GID:
             out = self.map_sc_gid_to_sc_point_gid(gid)
-        elif source == 'sc_gid':
+        elif source == SupplyCurveField.SC_GID:
             out = self.map_sc_point_gid_to_sc_gid(gid)
-        elif source == 'upwind':
+        elif source == "upwind":
             out = self.map_upwind(gid)
-        elif source == 'downwind':
+        elif source == "downwind":
             out = self.map_downwind(gid)
         else:
-            msg = ("{} must be: 'sc_gid', 'sc_point_gid',  or 'upwind', "
-                   "'downwind'".format(source))
+            msg = ("{} must be: {}, {},  or 'upwind', "
+                   "'downwind'".format(source, SupplyCurveField.SC_GID,
+                                       SupplyCurveField.SC_POINT_GID))
             logger.error(msg)
             raise ValueError(msg)
 
         return out
 
     @property
     def mask(self):
@@ -129,17 +139,17 @@
         """
         Un-masked sc_gids
 
         Returns
         -------
         ndarray
         """
-        sc_gids = \
-            np.concatenate([self._sc_point_gids[gid]
-                            for gid in self.sc_point_gids])
+        sc_gids = np.concatenate(
+            [self._sc_point_gids[gid] for gid in self.sc_point_gids]
+        )
 
         return sc_gids
 
     @staticmethod
     def _parse_table(table):
         """
         Extract features and their capacity from supply curve transmission
@@ -177,16 +187,18 @@
         Returns
         -------
         wind_dirs : pandas.DataFrame
             Neighboring supply curve point gids and power-rose value at each
             cardinal direction for each sc point gid
         """
         wind_dirs = cls._parse_table(wind_dirs)
+        wind_dirs = wind_dirs.rename(
+            columns=SupplyCurveField.map_from_legacy())
 
-        wind_dirs = wind_dirs.set_index('sc_point_gid')
+        wind_dirs = wind_dirs.set_index(SupplyCurveField.SC_POINT_GID)
         columns = [c for c in wind_dirs if c.endswith(('_gid', '_pr'))]
         wind_dirs = wind_dirs[columns]
 
         return wind_dirs
 
     @classmethod
     def _parse_sc_points(cls, sc_points, offshore=False):
@@ -208,29 +220,33 @@
             sc_gid to sc_point_gid mapping
         sc_point_gids : pandas.DataFrame
             sc_point_gid to sc_gid mapping
         mask : ndarray
             Mask array to mask excluded sc_point_gids
         """
         sc_points = cls._parse_table(sc_points)
-        if 'offshore' in sc_points and not offshore:
+        sc_points = sc_points.rename(
+            columns=SupplyCurveField.map_from_legacy())
+        if SupplyCurveField.OFFSHORE in sc_points and not offshore:
             logger.debug('Not including offshore supply curve points in '
                          'CompetitiveWindFarm')
-            mask = sc_points['offshore'] == 0
+            mask = sc_points[SupplyCurveField.OFFSHORE] == 0
             sc_points = sc_points.loc[mask]
 
-        mask = np.ones(int(1 + sc_points['sc_point_gid'].max()), dtype=bool)
+        mask = np.ones(int(1 + sc_points[SupplyCurveField.SC_POINT_GID].max()),
+                       dtype=bool)
 
-        sc_points = sc_points[['sc_gid', 'sc_point_gid']]
-        sc_gids = sc_points.set_index('sc_gid')
+        sc_points = sc_points[[SupplyCurveField.SC_GID,
+                               SupplyCurveField.SC_POINT_GID]]
+        sc_gids = sc_points.set_index(SupplyCurveField.SC_GID)
         sc_gids = {k: int(v[0]) for k, v in sc_gids.iterrows()}
 
-        sc_point_gids = \
-            sc_points.groupby('sc_point_gid')['sc_gid'].unique().to_frame()
-        sc_point_gids = {int(k): v['sc_gid']
+        groups = sc_points.groupby(SupplyCurveField.SC_POINT_GID)
+        sc_point_gids = groups[SupplyCurveField.SC_GID].unique().to_frame()
+        sc_point_gids = {int(k): v[SupplyCurveField.SC_GID]
                          for k, v in sc_point_gids.iterrows()}
 
         return sc_gids, sc_point_gids, mask
 
     @staticmethod
     def _get_neighbors(wind_dirs, n_dirs=2):
         """
@@ -247,27 +263,38 @@
         Returns
         -------
         upwind : pandas.DataFrame
             Upwind neighbor gids for n prominent wind directions
         downwind : pandas.DataFrame
             Downwind neighbor gids for n prominent wind directions
         """
-        cols = [c for c in wind_dirs
-                if (c.endswith('_gid') and not c.startswith('sc'))]
-        directions = [c.split('_')[0] for c in cols]
+        cols = [
+            c
+            for c in wind_dirs
+            if (c.endswith("_gid") and not c.startswith("sc"))
+        ]
+        directions = [c.split("_")[0] for c in cols]
         upwind_gids = wind_dirs[cols].values
 
-        cols = ['{}_pr'.format(d) for d in directions]
+        cols = ["{}_pr".format(d) for d in directions]
         neighbor_pr = wind_dirs[cols].values
 
         neighbors = np.argsort(neighbor_pr)[:, :n_dirs]
         upwind_gids = np.take_along_axis(upwind_gids, neighbors, axis=1)
 
-        downwind_map = {'N': 'S', 'NE': 'SW', 'E': 'W', 'SE': 'NW', 'S': 'N',
-                        'SW': 'NE', 'W': 'E', 'NW': 'SE'}
+        downwind_map = {
+            "N": "S",
+            "NE": "SW",
+            "E": "W",
+            "SE": "NW",
+            "S": "N",
+            "SW": "NE",
+            "W": "E",
+            "NW": "SE",
+        }
         cols = ["{}_gid".format(downwind_map[d]) for d in directions]
         downwind_gids = wind_dirs[cols].values
         downwind_gids = np.take_along_axis(downwind_gids, neighbors, axis=1)
 
         downwind = {}
         upwind = {}
         for i, gid in enumerate(wind_dirs.index.values):
@@ -334,14 +361,15 @@
         """
         Map given sc_point_gid to upwind neighbors
 
         Parameters
         ----------
         sc_point_gid : int
             Supply point curve gid to get upwind neighbors
+
         Returns
         -------
         int | list
             upwind neighborings
         """
         return self._upwind[sc_point_gid]
 
@@ -349,14 +377,15 @@
         """
         Map given sc_point_gid to downwind neighbors
 
         Parameters
         ----------
         sc_point_gid : int
             Supply point curve gid to get downwind neighbors
+
         Returns
         -------
         int | list
             downwind neighborings
         """
         return self._downwind[sc_point_gid]
 
@@ -379,16 +408,17 @@
             self._mask[sc_point_gid] = False
             out = True
         else:
             out = False
 
         return out
 
-    def remove_noncompetitive_farm(self, sc_points, sort_on='total_lcoe',
-                                   downwind=False):
+    def remove_noncompetitive_farm(
+        self, sc_points, sort_on="total_lcoe", downwind=False
+    ):
         """
         Remove neighboring sc points for given number of prominent wind
         directions
 
         Parameters
         ----------
         sc_points : pandas.DataFrame | str
@@ -403,42 +433,53 @@
         Returns
         -------
         sc_points : pandas.DataFrame
             Updated supply curve points after removing non-competative
             wind farms
         """
         sc_points = self._parse_table(sc_points)
-        if 'offshore' in sc_points and not self._offshore:
-            mask = sc_points['offshore'] == 0
+        sc_points = sc_points.rename(
+            columns=SupplyCurveField.map_from_legacy())
+        if SupplyCurveField.OFFSHORE in sc_points and not self._offshore:
+            mask = sc_points[SupplyCurveField.OFFSHORE] == 0
             sc_points = sc_points.loc[mask]
 
         sc_points = sc_points.sort_values(sort_on)
 
-        sc_point_gids = sc_points['sc_point_gid'].values.astype(int)
+        sc_point_gids = sc_points[SupplyCurveField.SC_POINT_GID].values
+        sc_point_gids = sc_point_gids.astype(int)
 
         for i in range(len(sc_points)):
             gid = sc_point_gids[i]
             if self.mask[gid]:
-                upwind_gids = self['upwind', gid]
+                upwind_gids = self["upwind", gid]
                 for n in upwind_gids:
                     self.exclude_sc_point_gid(n)
 
                 if downwind:
-                    downwind_gids = self['downwind', gid]
+                    downwind_gids = self["downwind", gid]
                     for n in downwind_gids:
                         self.exclude_sc_point_gid(n)
 
         sc_gids = self.sc_gids
-        mask = sc_points['sc_gid'].isin(sc_gids)
+        mask = sc_points[SupplyCurveField.SC_GID].isin(sc_gids)
 
         return sc_points.loc[mask].reset_index(drop=True)
 
     @classmethod
-    def run(cls, wind_dirs, sc_points, n_dirs=2, offshore=False,
-            sort_on='total_lcoe', downwind=False, out_fpath=None):
+    def run(
+        cls,
+        wind_dirs,
+        sc_points,
+        n_dirs=2,
+        offshore=False,
+        sort_on="total_lcoe",
+        downwind=False,
+        out_fpath=None,
+    ):
         """
         Exclude given number of neighboring Supply Point gids based on most
         prominent wind directions
 
         Parameters
         ----------
         wind_dirs : pandas.DataFrame | str
@@ -465,14 +506,15 @@
         Returns
         -------
         sc_points : pandas.DataFrame
             Updated supply curve points after removing non-competative
             wind farms
         """
         cwf = cls(wind_dirs, sc_points, n_dirs=n_dirs, offshore=offshore)
-        sc_points = cwf.remove_noncompetitive_farm(sc_points, sort_on=sort_on,
-                                                   downwind=downwind)
+        sc_points = cwf.remove_noncompetitive_farm(
+            sc_points, sort_on=sort_on, downwind=downwind
+        )
 
         if out_fpath is not None:
             sc_points.to_csv(out_fpath, index=False)
 
         return sc_points
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/exclusions.py` & `NREL-reV-0.8.9/reV/supply_curve/exclusions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 Generate reV inclusion mask from exclusion layers
 """
 import logging
-import numpy as np
-from scipy import ndimage
 from warnings import warn
 
+import numpy as np
 from rex.utilities.loggers import log_mem
-from reV.handlers.exclusions import ExclusionLayers
-from reV.utilities.exceptions import ExclusionLayerError
-from reV.utilities.exceptions import SupplyCurveInputError
+from scipy import ndimage
+
+from reV.handlers.exclusions import ExclusionLayers, LATITUDE, LONGITUDE
+from reV.utilities.exceptions import ExclusionLayerError, SupplyCurveInputError
 
 logger = logging.getLogger(__name__)
 
 
 class LayerMask:
     """
     Class to convert exclusion layer to inclusion layer mask
@@ -28,14 +28,15 @@
                  include_weights=None,
                  force_include_values=None,
                  force_include_range=None,
                  use_as_weights=False,
                  weight=1.0,
                  exclude_nodata=False,
                  nodata_value=None,
+                 extent=None,
                  **kwargs):
         """
         Parameters
         ----------
         layer : str
             Layer name.
         exclude_values : int | float | list, optional
@@ -45,47 +46,52 @@
               `exclude_range`, `include_values`, `include_range`,
               `include_weights`, `force_include_values`, and
               `force_include_range` are all mutually exclusive. Users
               should supply value(s) for exactly one of these arguments.
 
             By default, ``None``.
         exclude_range : list | tuple, optional
-            Two-item list of (min threshold, max threshold) for values
-            to exclude. Mutually exclusive with other inputs - see info
-            in the description of  `exclude_values`.
-            By default, ``None``.
+            Two-item list of [min threshold, max threshold] (ends are
+            inclusive) for values to exclude. Mutually exclusive
+            with other inputs (see info in the description of
+            `exclude_values`). By default, ``None``.
         include_values : int | float | list, optional
             Single value or list of values to include. Mutually
-            exclusive with other inputs - see info in the description of
-            `exclude_values`. By default, ``None``.
+            exclusive with other inputs (see info in the description of
+            `exclude_values`). By default, ``None``.
         include_range : list | tuple, optional
-            Two-item list of (min threshold, max threshold) for values
-            to include. Mutually exclusive with other inputs - see info
-            in the description of  `exclude_values`.
-            By default, ``None``.
+            Two-item list of [min threshold, max threshold] (ends are
+            inclusive) for values to include. Mutually exclusive with
+            other inputs (see info in the description of
+            `exclude_values`). By default, ``None``.
         include_weights : dict, optional
             A dictionary of ``{value: weight}`` pairs, where the
             ``value`` in the layer that should be included with the
-            given ``weight``. Mutually exclusive with other inputs - see
-            info in the description of  `exclude_values`.
+            given ``weight``. Mutually exclusive with other inputs (see
+            info in the description of  `exclude_values`).
             By default, ``None``.
         force_include_values : int | float | list, optional
-            Force the inclusion of the given value(s). Mutually
-            exclusive with other inputs - see info in the description of
-            `exclude_values`. By default, ``None``.
+            Force the inclusion of the given value(s). This input
+            completely replaces anything provided as `include_values`
+            and is mutually exclusive with other inputs (eee info in
+            the description of `exclude_values`). By default, ``None``.
         force_include_range : list | tuple, optional
             Force the inclusion of given values in the range
-            (min threshold, max threshold). Mutually exclusive with
-            other inputs - see info in the description of
-            `exclude_values`. By default, ``None``.
+            [min threshold, max threshold] (ends are inclusive). This
+            input completely replaces anything provided as
+            `include_range` and is mutually exclusive with other inputs
+            (see info in the description of `exclude_values`).
+            By default, ``None``.
         use_as_weights : bool, optional
-            Option to use layer as final inclusion weights. If ``True``,
-            all inclusion/exclusions specifications for the layer are
-            ignored and the raw values (scaled by the `weight` input)
-            are used as weights. By default, ``False``.
+            Option to use layer as final inclusion weights (i.e.
+            1 = fully included, 0.75 = 75% included, 0.5 = 50% included,
+            etc.). If ``True``, all inclusion/exclusions specifications
+            for the layer are ignored and the raw values (scaled by the
+            `weight` input) are used as inclusion weights.
+            By default, ``False``.
         weight : float, optional
             Weight applied to exclusion layer after it is calculated.
             Can be used, for example, to turn a binary exclusion layer
             (i.e. data with 0 or 1 values and ``exclude_values=1``
             input) into partial exclusions by setting the weight to
             a fraction (e.g. 0.5 for 50% exclusions). By default, ``1``.
         exclude_nodata : bool, optional
@@ -94,14 +100,46 @@
             :class:`reV.supply_curve.exclusions.ExclusionMask`.
             By default, ``False``.
         nodata_value : int | float, optional
             Nodata value for the layer. If ``None``, the value will be
             inferred when LayerMask is added to
             :class:`reV.supply_curve.exclusions.ExclusionMask`.
             By default, ``None``.
+        extent : dict, optional
+            Optional dictionary with values that can be used to
+            initialize this class (i.e. `layer`, `exclude_values`,
+            `include_range`, etc.). This dictionary should contain the
+            specifications to create a boolean mask that defines the
+            extent to which the original mask should be applied.
+            For example, suppose you specify the input the following
+            way:
+
+                input_dict = {
+                    "viewsheds": {
+                        "exclude_values": 1,
+                        "extent": {
+                            "layer": "federal_parks",
+                            "include_range": [1, 5]
+                        }
+                    }
+                }
+
+                for layer_name, kwargs in input_dict.items():
+                    layer = LayerMask(layer_name, **kwargs)
+                    ...
+
+            This would mean that you are masking out all viewshed layer
+            values equal to 1, **but only where the "federal_parks"
+            layer is equal to 1, 2, 3, 4, or 5**. Outside of these
+            regions (i.e. outside of federal park regions), the viewshed
+            exclusion is **NOT** applied. If the extent mask created by
+            these options is not boolean, an error is thrown (i.e. do
+            not specify `weight` or `use_as_weights`).
+            By default ``None``, which applies the original layer mask
+            to the full extent.
         **kwargs
             Optional inputs to maintain legacy kwargs of ``inclusion_*``
             instead of ``include_*``.
         """
 
         self._name = layer
         self._exclude_values = exclude_values
@@ -121,21 +159,22 @@
             self._force_include = True
 
         self._as_weights = use_as_weights
         self._exclude_nodata = exclude_nodata
         self.nodata_value = nodata_value
 
         if weight > 1 or weight < 0:
-            msg = ('Invalide weight ({}) provided for layer {}:'
+            msg = ('Invalid weight ({}) provided for layer {}:'
                    '\nWeight must fall between 0 and 1!'.format(weight, layer))
             logger.error(msg)
             raise ValueError(msg)
 
         self._weight = weight
         self._mask_type = self._check_mask_type()
+        self.extent = LayerMask(**extent) if extent is not None else None
 
     def __repr__(self):
         msg = ('{} for "{}" exclusion, of type "{}"'
                .format(self.__class__.__name__, self.name, self.mask_type))
 
         return msg
 
@@ -203,16 +242,15 @@
         if 'excl' in self.mask_type:
             range_var = self._exclude_range
         else:
             range_var = self._include_range
 
         if all(isinstance(x, (int, float)) for x in range_var):
             return min(range_var)
-        else:
-            return range_var[0]
+        return range_var[0]
 
     @property
     def max_value(self):
         """Maximum value to include/exclude if include_range or exclude_range
         was input.
 
         Returns
@@ -222,16 +260,15 @@
         if 'excl' in self.mask_type:
             range_var = self._exclude_range
         else:
             range_var = self._include_range
 
         if all(isinstance(x, (int, float)) for x in range_var):
             return max(range_var)
-        else:
-            return range_var[1]
+        return range_var[1]
 
     @property
     def exclude_values(self):
         """
         Values to exclude
 
         Returns
@@ -327,15 +364,15 @@
 
     def _check_mask_type(self):
         """
         Ensure that the initialization arguments are valid and not
         contradictory
 
         Returns
-        ------
+        -------
         mask : str
             Mask type
         """
         mask = None
         if not self._as_weights:
             masks = {'include_range': any(i is not None
                                           for i in self._include_range),
@@ -351,14 +388,24 @@
                     else:
                         msg = ('Only one approach can be used to create the '
                                'inclusion mask, but you supplied {} and {}'
                                .format(mask, k))
                         logger.error(msg)
                         raise ExclusionLayerError(msg)
 
+            if mask is None:
+                msg = ('Exactly one approach must be specified to create the '
+                       'inclusion mask for layer {!r}! Please specify one of: '
+                       '`exclude_values`, `exclude_range`, `include_values`, '
+                       '`include_range`, `include_weights`, '
+                       '`force_include_values`, or `force_include_range`.'
+                       .format(self.name))
+                logger.error(msg)
+                raise ExclusionLayerError(msg)
+
         if mask == 'include_weights' and self._weight < 1:
             msg = ("Values are individually weighted when using "
                    "'include_weights', the supplied weight of {} will be "
                    "ignored!".format(self._weight))
             self._weight = 1
             logger.warning(msg)
             warn(msg)
@@ -636,15 +683,15 @@
     def excl_h5(self):
         """
         Open ExclusionLayers instance
 
         Returns
         -------
         _excl_h5 : ExclusionLayers
-         """
+        """
         return self._excl_h5
 
     @property
     def excl_layers(self):
         """
         List of available exclusion layers in exclusions .h5
 
@@ -661,26 +708,26 @@
     def layer_names(self):
         """
         List of layers to combines
 
         Returns
         -------
         list
-         """
+        """
         return self._layers.keys()
 
     @property
     def layers(self):
         """
         List of LayerMask instances for each exclusion layer to combine
 
         Returns
         -------
          list
-         """
+        """
         return self._layers.values()
 
     @property
     def mask(self):
         """
         Inclusion mask for entire exclusion domain
 
@@ -696,26 +743,26 @@
         """
         Latitude coordinates array
 
         Returns
         -------
         ndarray
         """
-        return self.excl_h5['latitude']
+        return self.excl_h5[LATITUDE]
 
     @property
     def longitude(self):
         """
         Longitude coordinates array
 
         Returns
         -------
         ndarray
         """
-        return self.excl_h5['longitude']
+        return self.excl_h5[LONGITUDE]
 
     def add_layer(self, layer, replace=False):
         """
         Add layer to be combined
 
         Parameters
         ----------
@@ -884,42 +931,62 @@
             else:
                 ones_shape += (s, )
 
         mask = np.ones(ones_shape, dtype='float32')
 
         return mask
 
-    def _force_include(self, mask, layers, ds_slice):
-        """
-        Apply force inclusion layers
+    def _add_layer_to_mask(self, mask, layer, ds_slice, check_layers,
+                           combine_func):
+        """Add layer mask to full mask."""
+        layer_mask = self._compute_layer_mask(layer, ds_slice, check_layers)
+        if mask is None:
+            return layer_mask
+
+        return combine_func(mask, layer_mask, dtype='float32')
+
+    def _compute_layer_mask(self, layer, ds_slice, check_layers=False):
+        """Compute mask for single layer, including extent."""
+        layer_mask = self._masked_layer_data(layer, ds_slice)
+        layer_mask = self._apply_layer_mask_extent(layer, layer_mask, ds_slice)
+
+        logger.debug('Computed exclusions {} for {}. Layer has average value '
+                     'of {:.2f}.'
+                     .format(layer, ds_slice, layer_mask.mean()))
+        log_mem(logger, log_level='DEBUG')
 
-        Parameters
-        ----------
-        mask : ndarray | None
-            Mask to apply force inclusion layers to
-        layers : list
-            List of force inclusion layers
-        ds_slice : int | slice | list | ndarray
-            What to extract from ds, each arg is for a sequential axis.
-            For example, (slice(0, 64), slice(0, 64)) will extract a 64x64
-            exclusions mask.
-        """
-        for layer in layers:
-            layer_slice = (layer.name, ) + ds_slice
-            layer_mask = layer[self.excl_h5[layer_slice]]
-            logger.debug('Computing forced inclusions for {}. Layer has '
-                         'average value of {:.2f}'
-                         .format(layer, layer_mask.mean()))
-            log_mem(logger, log_level='DEBUG')
-            if mask is None:
-                mask = layer_mask
-            else:
-                mask = np.maximum(mask, layer_mask, dtype='float32')
+        if check_layers and not layer_mask.any():
+            msg = "Layer {} is fully excluded!".format(layer.name)
+            logger.error(msg)
+            raise ExclusionLayerError(msg)
 
-        return mask
+        return layer_mask
+
+    def _apply_layer_mask_extent(self, layer, layer_mask, ds_slice):
+        """Apply extent to layer mask, if any."""
+        if layer.extent is None:
+            return layer_mask
+
+        layer_extent = self._masked_layer_data(layer.extent, ds_slice)
+        if not np.array_equal(layer_extent, layer_extent.astype(bool)):
+            msg = ("Extent layer must be boolean (i.e. 0 and 1 values "
+                   "only)! Please check your extent definition for layer "
+                   "{} to ensure you are producing a boolean layer!"
+                   .format(layer.name))
+            logger.error(msg)
+            raise ExclusionLayerError(msg)
+
+        logger.debug("Filtering mask for layer %s down to specified extent",
+                     layer.name)
+        layer_mask = np.where(layer_extent, layer_mask, 1)
+        return layer_mask
+
+    def _masked_layer_data(self, layer, ds_slice):
+        """Extract masked data for layer."""
+        return layer[self.excl_h5[(layer.name, ) + ds_slice]]
 
     def _generate_mask(self, *ds_slice, check_layers=False):
         """
         Generate multiplicative inclusion mask from exclusion layers.
 
         Parameters
         ----------
@@ -946,35 +1013,21 @@
 
         if self.layers:
             force_include = []
             for layer in self.layers:
                 if layer.force_include:
                     force_include.append(layer)
                 else:
-                    layer_slice = (layer.name, ) + ds_slice
-                    layer_mask = layer[self.excl_h5[layer_slice]]
-
-                    logger.debug('Computed exclusions {} for {}. '
-                                 'Layer has average value of {:.2f}.'
-                                 .format(layer, ds_slice, layer_mask.mean()))
-                    log_mem(logger, log_level='DEBUG')
-
-                    if check_layers and not layer_mask.any():
-                        msg = ("Layer {} is fully excluded!"
-                               .format(layer.name))
-                        logger.error(msg)
-                        raise ExclusionLayerError(msg)
-
-                    if mask is None:
-                        mask = layer_mask
-                    else:
-                        mask = np.minimum(mask, layer_mask, dtype='float32')
-
-            if force_include:
-                mask = self._force_include(mask, force_include, ds_slice)
+                    mask = self._add_layer_to_mask(mask, layer, ds_slice,
+                                                   check_layers,
+                                                   combine_func=np.minimum)
+            for layer in force_include:
+                mask = self._add_layer_to_mask(mask, layer, ds_slice,
+                                               check_layers,
+                                               combine_func=np.maximum)
 
             if self._min_area is not None:
                 mask = self._area_filter(mask, self._min_area,
                                          self._excl_h5.pixel_area,
                                          kernel=self._kernel)
                 mask = mask[sub_slice]
         else:
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/extent.py` & `NREL-reV-0.8.9/reV/supply_curve/extent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 reV supply curve extent
 """
+
 import logging
+
 import numpy as np
 import pandas as pd
+from rex.utilities.utilities import get_chunk_ranges
 
-from reV.handlers.exclusions import ExclusionLayers
+from reV.handlers.exclusions import LATITUDE, LONGITUDE, ExclusionLayers
+from reV.utilities import SupplyCurveField
 from reV.utilities.exceptions import SupplyCurveError, SupplyCurveInputError
 
-from rex.utilities.utilities import get_chunk_ranges
-
 logger = logging.getLogger(__name__)
 
 
 class SupplyCurveExtent:
     """Supply curve full extent framework. This class translates the 90m
     exclusion grid to the aggregated supply curve resolution."""
 
@@ -27,34 +29,39 @@
             ExclusionLayers. The exclusions dictate the SC analysis extent.
         resolution : int
             Number of exclusion points per SC point along an axis.
             This number**2 is the total number of exclusion points per
             SC point.
         """
 
-        logger.debug('Initializing SupplyCurveExtent with res {} from: {}'
-                     .format(resolution, f_excl))
+        logger.debug(
+            "Initializing SupplyCurveExtent with res {} from: {}".format(
+                resolution, f_excl
+            )
+        )
 
         if not isinstance(resolution, int):
-            raise SupplyCurveInputError('Supply Curve resolution needs to be '
-                                        'an integer but received: {}'
-                                        .format(type(resolution)))
+            raise SupplyCurveInputError(
+                "Supply Curve resolution needs to be "
+                "an integer but received: {}".format(type(resolution))
+            )
 
         if isinstance(f_excl, (str, list, tuple)):
             self._excl_fpath = f_excl
             self._excls = ExclusionLayers(f_excl)
         elif isinstance(f_excl, ExclusionLayers):
             self._excl_fpath = f_excl.h5_file
             self._excls = f_excl
         else:
-            raise SupplyCurveInputError('SupplyCurvePoints needs an '
-                                        'exclusions file path, or '
-                                        'ExclusionLayers handler but '
-                                        'received: {}'
-                                        .format(type(f_excl)))
+            raise SupplyCurveInputError(
+                "SupplyCurvePoints needs an "
+                "exclusions file path, or "
+                "ExclusionLayers handler but "
+                "received: {}".format(type(f_excl))
+            )
 
         self._excl_shape = self.exclusions.shape
         # limit the resolution to the exclusion shape.
         self._res = int(np.min(list(self.excl_shape) + [resolution]))
 
         self._n_rows = None
         self._n_cols = None
@@ -63,21 +70,23 @@
         self._excl_row_slices = None
         self._excl_col_slices = None
         self._latitude = None
         self._longitude = None
         self._points = None
 
         self._sc_col_ind, self._sc_row_ind = np.meshgrid(
-            np.arange(self.n_cols), np.arange(self.n_rows))
+            np.arange(self.n_cols), np.arange(self.n_rows)
+        )
         self._sc_col_ind = self._sc_col_ind.flatten()
         self._sc_row_ind = self._sc_row_ind.flatten()
 
-        logger.debug('Initialized SupplyCurveExtent with shape {} from '
-                     'exclusions with shape {}'
-                     .format(self.shape, self.excl_shape))
+        logger.debug(
+            "Initialized SupplyCurveExtent with shape {} from "
+            "exclusions with shape {}".format(self.shape, self.excl_shape)
+        )
 
     def __len__(self):
         """Total number of supply curve points."""
         return self.n_rows * self.n_cols
 
     def __enter__(self):
         return self
@@ -86,16 +95,18 @@
         self.close()
         if type is not None:
             raise
 
     def __getitem__(self, gid):
         """Get SC extent meta data corresponding to an SC point gid."""
         if gid >= len(self):
-            raise KeyError('SC extent with {} points does not contain SC '
-                           'point gid {}.'.format(len(self), gid))
+            raise KeyError(
+                "SC extent with {} points does not contain SC "
+                "point gid {}.".format(len(self), gid)
+            )
 
         return self.points.loc[gid]
 
     def close(self):
         """Close all file handlers."""
         self._excls.close()
 
@@ -176,16 +187,17 @@
         -------
         _rows_of_excl : list
             List representing the supply curve points rows. Each list entry
             contains the exclusion row indices that are included in the sc
             point.
         """
         if self._rows_of_excl is None:
-            self._rows_of_excl = self._chunk_excl(self.excl_rows,
-                                                  self.resolution)
+            self._rows_of_excl = self._chunk_excl(
+                self.excl_rows, self.resolution
+            )
 
         return self._rows_of_excl
 
     @property
     def cols_of_excl(self):
         """List representing the supply curve points columns and which
         exclusions columns belong to each supply curve column.
@@ -194,16 +206,17 @@
         -------
         _cols_of_excl : list
             List representing the supply curve points columns. Each list entry
             contains the exclusion column indices that are included in the sc
             point.
         """
         if self._cols_of_excl is None:
-            self._cols_of_excl = self._chunk_excl(self.excl_cols,
-                                                  self.resolution)
+            self._cols_of_excl = self._chunk_excl(
+                self.excl_cols, self.resolution
+            )
 
         return self._cols_of_excl
 
     @property
     def excl_row_slices(self):
         """
         List representing the supply curve points rows and which
@@ -213,16 +226,17 @@
         -------
         _excl_row_slices : list
             List representing the supply curve points rows. Each list entry
             contains the exclusion row slice that are included in the sc
             point.
         """
         if self._excl_row_slices is None:
-            self._excl_row_slices = self._excl_slices(self.excl_rows,
-                                                      self.resolution)
+            self._excl_row_slices = self._excl_slices(
+                self.excl_rows, self.resolution
+            )
 
         return self._excl_row_slices
 
     @property
     def excl_col_slices(self):
         """
         List representing the supply curve points cols and which
@@ -232,16 +246,17 @@
         -------
         _excl_col_slices : list
             List representing the supply curve points cols. Each list entry
             contains the exclusion col slice that are included in the sc
             point.
         """
         if self._excl_col_slices is None:
-            self._excl_col_slices = self._excl_slices(self.excl_cols,
-                                                      self.resolution)
+            self._excl_col_slices = self._excl_slices(
+                self.excl_cols, self.resolution
+            )
 
         return self._excl_col_slices
 
     @property
     def n_rows(self):
         """Get the number of supply curve grid rows.
 
@@ -278,24 +293,25 @@
         -------
         ndarray
         """
         if self._latitude is None:
             lats = []
             lons = []
 
-            sc_cols, sc_rows = np.meshgrid(np.arange(self.n_cols),
-                                           np.arange(self.n_rows))
+            sc_cols, sc_rows = np.meshgrid(
+                np.arange(self.n_cols), np.arange(self.n_rows)
+            )
             for r, c in zip(sc_rows.flatten(), sc_cols.flatten()):
                 r = self.excl_row_slices[r]
                 c = self.excl_col_slices[c]
-                lats.append(self.exclusions['latitude', r, c].mean())
-                lons.append(self.exclusions['longitude', r, c].mean())
+                lats.append(self.exclusions[LATITUDE, r, c].mean())
+                lons.append(self.exclusions[LONGITUDE, r, c].mean())
 
-            self._latitude = np.array(lats, dtype='float32')
-            self._longitude = np.array(lons, dtype='float32')
+            self._latitude = np.array(lats, dtype="float32")
+            self._longitude = np.array(lons, dtype="float32")
 
         return self._latitude
 
     @property
     def longitude(self):
         """
         Get supply curve point longitudes
@@ -304,24 +320,25 @@
         -------
         ndarray
         """
         if self._longitude is None:
             lats = []
             lons = []
 
-            sc_cols, sc_rows = np.meshgrid(np.arange(self.n_cols),
-                                           np.arange(self.n_rows))
+            sc_cols, sc_rows = np.meshgrid(
+                np.arange(self.n_cols), np.arange(self.n_rows)
+            )
             for r, c in zip(sc_rows.flatten(), sc_cols.flatten()):
                 r = self.excl_row_slices[r]
                 c = self.excl_col_slices[c]
-                lats.append(self.exclusions['latitude', r, c].mean())
-                lons.append(self.exclusions['longitude', r, c].mean())
+                lats.append(self.exclusions[LATITUDE, r, c].mean())
+                lons.append(self.exclusions[LONGITUDE, r, c].mean())
 
-            self._latitude = np.array(lats, dtype='float32')
-            self._longitude = np.array(lons, dtype='float32')
+            self._latitude = np.array(lats, dtype="float32")
+            self._longitude = np.array(lons, dtype="float32")
 
         return self._longitude
 
     @property
     def lat_lon(self):
         """
         2D array of lat, lon coordinates for all sc points
@@ -363,18 +380,22 @@
         Returns
         -------
         _points : pd.DataFrame
             Supply curve points with columns for attributes of each sc point.
         """
 
         if self._points is None:
-            self._points = pd.DataFrame({'row_ind': self.row_indices.copy(),
-                                         'col_ind': self.col_indices.copy()})
+            self._points = pd.DataFrame(
+                {
+                    "row_ind": self.row_indices.copy(),
+                    "col_ind": self.col_indices.copy(),
+                }
+            )
 
-            self._points.index.name = 'gid'  # sc_point_gid
+            self._points.index.name = SupplyCurveField.GID  # sc_point_gid
 
         return self._points
 
     @staticmethod
     def _chunk_excl(arr, resolution):
         """Split an array into a list of arrays with len == resolution.
 
@@ -432,16 +453,16 @@
         Returns
         -------
         row_ind : int
             Row index that the gid is located at in the sc grid.
         col_ind : int
             Column index that the gid is located at in the sc grid.
         """
-        row_ind = self.points.loc[gid, 'row_ind']
-        col_ind = self.points.loc[gid, 'col_ind']
+        row_ind = self.points.loc[gid, "row_ind"]
+        col_ind = self.points.loc[gid, "col_ind"]
         return row_ind, col_ind
 
     def get_excl_slices(self, gid):
         """Get the row and column slices of the exclusions grid corresponding
         to the supply curve point gid.
 
         Parameters
@@ -454,17 +475,18 @@
         row_slice : slice
             Exclusions grid row slice corresponding to the sc point gid.
         col_slice : slice
             Exclusions grid col slice corresponding to the sc point gid.
         """
 
         if gid >= len(self):
-            raise SupplyCurveError('Requested gid "{}" is out of bounds for '
-                                   'supply curve points with length "{}".'
-                                   .format(gid, len(self)))
+            raise SupplyCurveError(
+                'Requested gid "{}" is out of bounds for '
+                'supply curve points with length "{}".'.format(gid, len(self))
+            )
 
         row_slice = self.excl_row_slices[self.row_indices[gid]]
         col_slice = self.excl_col_slices[self.col_indices[gid]]
 
         return row_slice, col_slice
 
     def get_flat_excl_ind(self, gid):
@@ -555,17 +577,20 @@
             for c in self.excl_col_slices:
                 if np.any(tm[r, c] != -1):
                     valid_bool[gid] = 1
                 gid += 1
 
         valid_gids = np.where(valid_bool == 1)[0].astype(np.uint32)
 
-        logger.info('Found {} valid SC points out of {} total possible '
-                    '(valid SC points that map to valid resource gids)'
-                    .format(len(valid_gids), len(valid_bool)))
+        logger.info(
+            "Found {} valid SC points out of {} total possible "
+            "(valid SC points that map to valid resource gids)".format(
+                len(valid_gids), len(valid_bool)
+            )
+        )
 
         return valid_gids
 
     def get_slice_lookup(self, sc_point_gids):
         """
         Get exclusion slices for all requested supply curve point gids
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/points.py` & `NREL-reV-0.8.9/reV/supply_curve/points.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 """
 reV supply curve points frameworks.
 """
-from abc import ABC
+
 import logging
+from abc import ABC
+from warnings import warn
+
 import numpy as np
 import pandas as pd
-from warnings import warn
+from rex.multi_time_resource import MultiTimeResource
+from rex.resource import BaseResource, Resource
+from rex.utilities.utilities import jsonify_dict
 
 from reV.econ.economies_of_scale import EconomiesOfScale
 from reV.econ.utilities import lcoe_fcr
-from reV.handlers.exclusions import ExclusionLayers
+from reV.handlers.exclusions import LATITUDE, LONGITUDE, ExclusionLayers
 from reV.supply_curve.exclusions import ExclusionMask, ExclusionMaskFromDict
-from reV.utilities.exceptions import (SupplyCurveInputError,
-                                      EmptySupplyCurvePointError,
-                                      InputWarning,
-                                      FileInputError,
-                                      DataShapeError,
-                                      OutputWarning)
-
-from rex.resource import Resource, BaseResource
-from rex.multi_time_resource import MultiTimeResource
-from rex.utilities.utilities import jsonify_dict
+from reV.utilities import ResourceMetaField, SupplyCurveField
+from reV.utilities.exceptions import (
+    DataShapeError,
+    EmptySupplyCurvePointError,
+    FileInputError,
+    InputWarning,
+    OutputWarning,
+    SupplyCurveInputError,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractSupplyCurvePoint(ABC):
     """
     Abstract SC point based on only the point gid, SC shape, and resolution.
@@ -44,15 +48,16 @@
             This number**2 is the total number of exclusion points per
             SC point.
         """
 
         self._gid = gid
         self._resolution = resolution
         self._rows, self._cols = self._parse_slices(
-            gid, resolution, exclusion_shape)
+            gid, resolution, exclusion_shape
+        )
 
     @staticmethod
     def _ordered_unique(seq):
         """Get a list of unique values in the same order as the input sequence.
 
         Parameters
         ----------
@@ -94,15 +99,15 @@
 
         rows, cols = self.get_agg_slices(gid, exclusion_shape, resolution)
 
         return rows, cols
 
     @property
     def gid(self):
-        """supply curve point gid"""
+        """Supply curve point gid"""
         return self._gid
 
     @property
     def sc_point_gid(self):
         """
         Supply curve point gid
 
@@ -168,16 +173,18 @@
         super_shape = (nrows, ncols)
         arr = np.arange(nrows * ncols).reshape(super_shape)
         try:
             loc = np.where(arr == gid)
             row = loc[0][0]
             col = loc[1][0]
         except IndexError as exc:
-            msg = ('Gid {} out of bounds for extent shape {} and '
-                   'resolution {}.'.format(gid, shape, resolution))
+            msg = (
+                "Gid {} out of bounds for extent shape {} and "
+                "resolution {}.".format(gid, shape, resolution)
+            )
             raise IndexError(msg) from exc
 
         if row + 1 != nrows:
             row_slice = slice(row * resolution, (row + 1) * resolution)
         else:
             row_slice = slice(row * resolution, shape[0])
 
@@ -188,17 +195,26 @@
 
         return row_slice, col_slice
 
 
 class SupplyCurvePoint(AbstractSupplyCurvePoint):
     """Generic single SC point based on exclusions, resolution, and techmap"""
 
-    def __init__(self, gid, excl, tm_dset, excl_dict=None, inclusion_mask=None,
-                 resolution=64, excl_area=None, exclusion_shape=None,
-                 close=True):
+    def __init__(
+        self,
+        gid,
+        excl,
+        tm_dset,
+        excl_dict=None,
+        inclusion_mask=None,
+        resolution=64,
+        excl_area=None,
+        exclusion_shape=None,
+        close=True,
+    ):
         """
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
         excl : str | list | tuple | ExclusionMask
             Filepath(s) to exclusions h5 or ExclusionMask file handler.
@@ -241,16 +257,18 @@
         self._gids = self._parse_techmap(tm_dset)
         self._h5_gids = self._gids
         self._h5_gid_set = None
 
         self._incl_mask = inclusion_mask
         self._incl_mask_flat = None
         if inclusion_mask is not None:
-            msg = ('Bad inclusion mask input shape of {} with stated '
-                   'resolution of {}'.format(inclusion_mask.shape, resolution))
+            msg = (
+                "Bad inclusion mask input shape of {} with stated "
+                "resolution of {}".format(inclusion_mask.shape, resolution)
+            )
             assert len(inclusion_mask.shape) == 2, msg
             assert inclusion_mask.shape[0] <= resolution, msg
             assert inclusion_mask.shape[1] <= resolution, msg
             assert inclusion_mask.size == len(self._gids), msg
             self._incl_mask = inclusion_mask.copy()
 
         self._centroid = None
@@ -278,19 +296,20 @@
         if isinstance(excl, (str, list, tuple)):
             excl_fpath = excl
             exclusions = None
         elif isinstance(excl, ExclusionMask):
             excl_fpath = excl.excl_h5.h5_file
             exclusions = excl
         else:
-            raise SupplyCurveInputError('SupplyCurvePoints needs an '
-                                        'exclusions file path, or '
-                                        'ExclusionMask handler but '
-                                        'received: {}'
-                                        .format(type(excl)))
+            raise SupplyCurveInputError(
+                "SupplyCurvePoints needs an "
+                "exclusions file path, or "
+                "ExclusionMask handler but "
+                "received: {}".format(type(excl))
+            )
 
         return excl_fpath, exclusions
 
     def _parse_techmap(self, tm_dset):
         """Parse data from the tech map file (exclusions to resource mapping).
         Raise EmptySupplyCurvePointError if there are no valid resource points
         in this SC point.
@@ -308,17 +327,20 @@
             gids (native resource index) from the original resource data
             corresponding to the tech exclusions.
         """
         res_gids = self.exclusions.excl_h5[tm_dset, self.rows, self.cols]
         res_gids = res_gids.astype(np.int32).flatten()
 
         if (res_gids != -1).sum() == 0:
-            emsg = ('Supply curve point gid {} has no viable exclusion points '
-                    'based on exclusions file: "{}"'
-                    .format(self._gid, self._excl_fpath))
+            emsg = (
+                "Supply curve point gid {} has no viable exclusion points "
+                'based on exclusions file: "{}"'.format(
+                    self._gid, self._excl_fpath
+                )
+            )
             raise EmptySupplyCurvePointError(emsg)
 
         return res_gids
 
     def __enter__(self):
         return self
 
@@ -339,32 +361,33 @@
 
         Returns
         -------
         _excls : ExclusionMask
             ExclusionMask h5 handler object.
         """
         if self._excls is None:
-            self._excls = ExclusionMaskFromDict(self._excl_fpath,
-                                                layers_dict=self._excl_dict)
+            self._excls = ExclusionMaskFromDict(
+                self._excl_fpath, layers_dict=self._excl_dict
+            )
 
         return self._excls
 
     @property
     def centroid(self):
         """Get the supply curve point centroid coordinate.
 
         Returns
         -------
         centroid : tuple
             SC point centroid (lat, lon).
         """
 
         if self._centroid is None:
-            lats = self.exclusions.excl_h5['latitude', self.rows, self.cols]
-            lons = self.exclusions.excl_h5['longitude', self.rows, self.cols]
+            lats = self.exclusions.excl_h5[LATITUDE, self.rows, self.cols]
+            lons = self.exclusions.excl_h5[LONGITUDE, self.rows, self.cols]
             self._centroid = (lats.mean(), lons.mean())
 
         return self._centroid
 
     @property
     def pixel_area(self):
         """The area in km2 of a single exclusion pixel. If this value was not
@@ -434,16 +457,20 @@
             self._incl_mask = self.exclusions[self.rows, self.cols]
 
             # make sure exclusion pixels outside resource extent are excluded
             out_of_extent = self._gids.reshape(self._incl_mask.shape) == -1
             self._incl_mask[out_of_extent] = 0.0
 
             if self._incl_mask.max() > 1:
-                w = ('Exclusions data max value is > 1: {}'
-                     .format(self._incl_mask.max()), InputWarning)
+                w = (
+                    "Exclusions data max value is > 1: {}".format(
+                        self._incl_mask.max()
+                    ),
+                    InputWarning,
+                )
                 logger.warning(w)
                 warn(w)
 
         return self._incl_mask
 
     @property
     def include_mask_flat(self):
@@ -501,16 +528,17 @@
 
     def _check_excl(self):
         """
         Check to see if supply curve point is fully excluded
         """
 
         if all(self.include_mask_flat[self.bool_mask] == 0):
-            msg = ('Supply curve point gid {} is completely excluded!'
-                   .format(self._gid))
+            msg = "Supply curve point gid {} is completely excluded!".format(
+                self._gid
+            )
             raise EmptySupplyCurvePointError(msg)
 
     def exclusion_weighted_mean(self, arr, drop_nan=True):
         """
         Calc the exclusions-weighted mean value of an array of resource data.
 
         Parameters
@@ -526,26 +554,26 @@
         mean : float | np.ndarray
             Mean of arr masked by the binary exclusions then weighted by
             the non-zero exclusions. This will be a 1D numpy array if the
             input data is a 2D numpy array (averaged along axis=1)
         """
 
         if len(arr.shape) == 2:
-            x = arr[:, self._gids[self.bool_mask]].astype('float32')
+            x = arr[:, self._gids[self.bool_mask]].astype("float32")
             incl = self.include_mask_flat[self.bool_mask]
             x *= incl
             mean = x.sum(axis=1) / incl.sum()
 
         else:
-            x = arr[self._gids[self.bool_mask]].astype('float32')
+            x = arr[self._gids[self.bool_mask]].astype("float32")
             incl = self.include_mask_flat[self.bool_mask]
 
             if np.isnan(x).all():
                 return np.nan
-            elif drop_nan and np.isnan(x).any():
+            if drop_nan and np.isnan(x).any():
                 nan_mask = np.isnan(x)
                 x = x[~nan_mask]
                 incl = incl[~nan_mask]
 
             x *= incl
             mean = x.sum() / incl.sum()
 
@@ -596,28 +624,37 @@
 
         Returns
         -------
         agg : float
             Sum of arr masked by the binary exclusions
         """
         if len(arr.shape) == 2:
-            x = arr[:, self._gids[self.bool_mask]].astype('float32')
+            x = arr[:, self._gids[self.bool_mask]].astype("float32")
             ax = 1
         else:
-            x = arr[self._gids[self.bool_mask]].astype('float32')
+            x = arr[self._gids[self.bool_mask]].astype("float32")
             ax = 0
 
         x *= self.include_mask_flat[self.bool_mask]
         agg = x.sum(axis=ax)
 
         return agg
 
     @classmethod
-    def sc_mean(cls, gid, excl, tm_dset, data, excl_dict=None, resolution=64,
-                exclusion_shape=None, close=True):
+    def sc_mean(
+        cls,
+        gid,
+        excl,
+        tm_dset,
+        data,
+        excl_dict=None,
+        resolution=64,
+        exclusion_shape=None,
+        close=True,
+    ):
         """
         Compute exclusions weight mean for the sc point from data
 
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
@@ -645,24 +682,37 @@
             Flag to close object file handlers on exit
 
         Returns
         -------
         ndarray
             Exclusions weighted means of data for supply curve point
         """
-        kwargs = {"excl_dict": excl_dict, "resolution": resolution,
-                  "exclusion_shape": exclusion_shape, "close": close}
+        kwargs = {
+            "excl_dict": excl_dict,
+            "resolution": resolution,
+            "exclusion_shape": exclusion_shape,
+            "close": close,
+        }
         with cls(gid, excl, tm_dset, **kwargs) as point:
             means = point.exclusion_weighted_mean(data)
 
         return means
 
     @classmethod
-    def sc_sum(cls, gid, excl, tm_dset, data, excl_dict=None, resolution=64,
-               exclusion_shape=None, close=True):
+    def sc_sum(
+        cls,
+        gid,
+        excl,
+        tm_dset,
+        data,
+        excl_dict=None,
+        resolution=64,
+        exclusion_shape=None,
+        close=True,
+    ):
         """
         Compute the aggregate (sum) of data for the sc point
 
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
@@ -690,16 +740,20 @@
             Flag to close object file handlers on exit.
 
         Returns
         -------
         ndarray
             Sum / aggregation of data for supply curve point
         """
-        kwargs = {"excl_dict": excl_dict, "resolution": resolution,
-                  "exclusion_shape": exclusion_shape, "close": close}
+        kwargs = {
+            "excl_dict": excl_dict,
+            "resolution": resolution,
+            "exclusion_shape": exclusion_shape,
+            "close": close,
+        }
         with cls(gid, excl, tm_dset, **kwargs) as point:
             agg = point.aggregate(data)
 
         return agg
 
     @staticmethod
     def _mode(data):
@@ -714,17 +768,16 @@
         Returns
         -------
         float | int
             Mode of data
         """
         if not data.size:
             return None
-        else:
-            # pd series is more flexible with non-numeric than stats mode
-            return pd.Series(data).mode().values[0]
+        # pd series is more flexible with non-numeric than stats mode
+        return pd.Series(data).mode().values[0]
 
     @staticmethod
     def _categorize(data, incl_mult):
         """
         Extract the sum of inclusion scalar values (where 1 is
         included, 0 is excluded, and 0.7 is included with 70 percent of
         available land) for each unique (categorical value) in data
@@ -739,16 +792,18 @@
         Returns
         -------
         str
             Jsonified string of the dictionary mapping categorical values to
             total inclusions
         """
 
-        data = {category: float(incl_mult[(data == category)].sum())
-                for category in np.unique(data)}
+        data = {
+            category: float(incl_mult[(data == category)].sum())
+            for category in np.unique(data)
+        }
         data = jsonify_dict(data)
 
         return data
 
     @classmethod
     def _agg_data_layer_method(cls, data, incl_mult, method):
         """Aggregate the data array using specified method.
@@ -766,41 +821,47 @@
             Aggregation method (mode, mean, max, min, sum, category)
 
         Returns
         -------
         data : float | int | str | None
             Result of applying method to data.
         """
-        method_func = {'mode': cls._mode,
-                       'mean': np.mean,
-                       'max': np.max,
-                       'min': np.min,
-                       'sum': np.sum,
-                       'category': cls._categorize}
+        method_func = {
+            "mode": cls._mode,
+            "mean": np.mean,
+            "max": np.max,
+            "min": np.min,
+            "sum": np.sum,
+            "category": cls._categorize,
+        }
 
         if data is not None:
             method = method.lower()
             if method not in method_func:
-                e = ('Cannot recognize data layer agg method: '
-                     '"{}". Can only {}'.format(method, list(method_func)))
+                e = (
+                    "Cannot recognize data layer agg method: "
+                    '"{}". Can only {}'.format(method, list(method_func))
+                )
                 logger.error(e)
                 raise ValueError(e)
 
             if len(data.shape) > 1:
                 data = data.flatten()
 
             if data.shape != incl_mult.shape:
-                e = ('Cannot aggregate data with shape that doesnt '
-                     'match excl mult!')
+                e = (
+                    "Cannot aggregate data with shape that doesnt "
+                    "match excl mult!"
+                )
                 logger.error(e)
                 raise DataShapeError(e)
 
-            if method == 'category':
-                data = method_func['category'](data, incl_mult)
-            elif method in ['mean', 'sum']:
+            if method == "category":
+                data = method_func["category"](data, incl_mult)
+            elif method in ["mean", "sum"]:
                 data = data * incl_mult
                 data = method_func[method](data)
             else:
                 data = method_func[method](data)
 
         return data
 
@@ -824,55 +885,70 @@
         summary : dict
             Dictionary of summary outputs for this sc point. A new entry for
             each data layer is added.
         """
 
         if data_layers is not None:
             for name, attrs in data_layers.items():
-                excl_fp = attrs.get('fpath', self._excl_fpath)
+                excl_fp = attrs.get("fpath", self._excl_fpath)
                 if excl_fp != self._excl_fpath:
-                    fh = ExclusionLayers(attrs['fpath'])
+                    fh = ExclusionLayers(attrs["fpath"])
                 else:
                     fh = self.exclusions.excl_h5
 
-                raw = fh[attrs['dset'], self.rows, self.cols]
-                nodata = fh.get_nodata_value(attrs['dset'])
+                raw = fh[attrs["dset"], self.rows, self.cols]
+                nodata = fh.get_nodata_value(attrs["dset"])
 
                 data = raw.flatten()[self.bool_mask]
                 incl_mult = self.include_mask_flat[self.bool_mask].copy()
 
                 if nodata is not None:
-                    valid_data_mask = (data != nodata)
+                    valid_data_mask = data != nodata
                     data = data[valid_data_mask]
                     incl_mult = incl_mult[valid_data_mask]
 
                     if not data.size:
-                        m = ('Data layer "{}" has no valid data for '
-                             'SC point gid {} because of exclusions '
-                             'and/or nodata values in the data layer.'
-                             .format(name, self._gid))
+                        m = (
+                            'Data layer "{}" has no valid data for '
+                            "SC point gid {} because of exclusions "
+                            "and/or nodata values in the data layer.".format(
+                                name, self._gid
+                            )
+                        )
                         logger.debug(m)
 
-                data = self._agg_data_layer_method(data, incl_mult,
-                                                   attrs['method'])
+                data = self._agg_data_layer_method(
+                    data, incl_mult, attrs["method"]
+                )
                 summary[name] = data
 
                 if excl_fp != self._excl_fpath:
                     fh.close()
 
         return summary
 
 
 class AggregationSupplyCurvePoint(SupplyCurvePoint):
     """Generic single SC point to aggregate data from an h5 file."""
 
-    def __init__(self, gid, excl, agg_h5, tm_dset,
-                 excl_dict=None, inclusion_mask=None,
-                 resolution=64, excl_area=None, exclusion_shape=None,
-                 close=True, gen_index=None, apply_exclusions=True):
+    def __init__(
+        self,
+        gid,
+        excl,
+        agg_h5,
+        tm_dset,
+        excl_dict=None,
+        inclusion_mask=None,
+        resolution=64,
+        excl_area=None,
+        exclusion_shape=None,
+        close=True,
+        gen_index=None,
+        apply_exclusions=True,
+    ):
         """
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
         excl : str | ExclusionMask
             Filepath to exclusions h5 or ExclusionMask file handler.
@@ -907,33 +983,40 @@
             Array of generation gids with array index equal to resource gid.
             Array value is -1 if the resource index was not used in the
             generation run.
         apply_exclusions : bool
             Flag to apply exclusions to the resource / generation gid's on
             initialization.
         """
-        super().__init__(gid, excl, tm_dset,
-                         excl_dict=excl_dict,
-                         inclusion_mask=inclusion_mask,
-                         resolution=resolution,
-                         excl_area=excl_area,
-                         exclusion_shape=exclusion_shape,
-                         close=close)
+        super().__init__(
+            gid,
+            excl,
+            tm_dset,
+            excl_dict=excl_dict,
+            inclusion_mask=inclusion_mask,
+            resolution=resolution,
+            excl_area=excl_area,
+            exclusion_shape=exclusion_shape,
+            close=close,
+        )
 
         self._h5_fpath, self._h5 = self._parse_h5_file(agg_h5)
 
         if gen_index is not None:
             self._gids, _ = self._map_gen_gids(self._gids, gen_index)
 
         self._h5_gids = self._gids
 
         if (self._h5_gids != -1).sum() == 0:
-            emsg = ('Supply curve point gid {} has no viable exclusion '
-                    'points based on exclusions file: "{}"'
-                    .format(self._gid, self._excl_fpath))
+            emsg = (
+                "Supply curve point gid {} has no viable exclusion "
+                'points based on exclusions file: "{}"'.format(
+                    self._gid, self._excl_fpath
+                )
+            )
             raise EmptySupplyCurvePointError(emsg)
 
         if apply_exclusions:
             self._apply_exclusions()
 
     @staticmethod
     def _parse_h5_file(h5):
@@ -958,19 +1041,20 @@
             h5_fpath = h5
             h5 = None
         elif issubclass(h5.__class__, BaseResource):
             h5_fpath = h5.h5_file
         elif issubclass(h5.__class__, MultiTimeResource):
             h5_fpath = h5.h5_files
         else:
-            raise SupplyCurveInputError('SupplyCurvePoints needs a '
-                                        '.h5 file path, or '
-                                        'Resource handler but '
-                                        'received: {}'
-                                        .format(type(h5)))
+            raise SupplyCurveInputError(
+                "SupplyCurvePoints needs a "
+                ".h5 file path, or "
+                "Resource handler but "
+                "received: {}".format(type(h5))
+            )
 
         return h5_fpath, h5
 
     def _apply_exclusions(self):
         """Apply exclusions by masking the generation and resource gid arrays.
         This removes all res/gen entries that are masked by the exclusions or
         resource bin."""
@@ -978,16 +1062,17 @@
         # exclusions mask is False where excluded
         exclude = self.include_mask_flat == 0
 
         self._gids[exclude] = -1
         self._h5_gids[exclude] = -1
 
         if (self._gids != -1).sum() == 0:
-            msg = ('Supply curve point gid {} is completely excluded!'
-                   .format(self._gid))
+            msg = "Supply curve point gid {} is completely excluded!".format(
+                self._gid
+            )
             raise EmptySupplyCurvePointError(msg)
 
     def close(self):
         """Close all file handlers."""
         if self._close:
             if self._excls is not None:
                 self._excls.close()
@@ -1028,105 +1113,136 @@
         h5 Resource handler object
 
         Returns
         -------
         _h5 : Resource
             Resource h5 handler object.
         """
-        if self._h5 is None and '*' in self._h5_fpath:
+        if self._h5 is None and "*" in self._h5_fpath:
             self._h5 = MultiTimeResource(self._h5_fpath)
         elif self._h5 is None:
             self._h5 = Resource(self._h5_fpath)
 
         return self._h5
 
     @property
     def country(self):
         """Get the SC point country based on the resource meta data."""
         country = None
-        if 'country' in self.h5.meta and self.county is not None:
+        county_not_none = self.county is not None
+        if ResourceMetaField.COUNTRY in self.h5.meta and county_not_none:
             # make sure country and county are coincident
-            counties = self.h5.meta.loc[self.h5_gid_set, 'county'].values
+            counties = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.COUNTY
+            ].values
             iloc = np.where(counties == self.county)[0][0]
-            country = self.h5.meta.loc[self.h5_gid_set, 'country'].values
+            country = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.COUNTRY
+            ].values
             country = country[iloc]
 
-        elif 'country' in self.h5.meta:
-            country = self.h5.meta.loc[self.h5_gid_set, 'country'].mode()
+        elif ResourceMetaField.COUNTRY in self.h5.meta:
+            country = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.COUNTRY
+            ].mode()
             country = country.values[0]
 
         return country
 
     @property
     def state(self):
         """Get the SC point state based on the resource meta data."""
         state = None
-        if 'state' in self.h5.meta and self.county is not None:
+        if ResourceMetaField.STATE in self.h5.meta and self.county is not None:
             # make sure state and county are coincident
-            counties = self.h5.meta.loc[self.h5_gid_set, 'county'].values
+            counties = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.COUNTY
+            ].values
             iloc = np.where(counties == self.county)[0][0]
-            state = self.h5.meta.loc[self.h5_gid_set, 'state'].values
+            state = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.STATE
+            ].values
             state = state[iloc]
 
-        elif 'state' in self.h5.meta:
-            state = self.h5.meta.loc[self.h5_gid_set, 'state'].mode()
+        elif ResourceMetaField.STATE in self.h5.meta:
+            state = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.STATE
+            ].mode()
             state = state.values[0]
 
         return state
 
     @property
     def county(self):
         """Get the SC point county based on the resource meta data."""
         county = None
-        if 'county' in self.h5.meta:
-            county = self.h5.meta.loc[self.h5_gid_set, 'county'].mode()
+        if ResourceMetaField.COUNTY in self.h5.meta:
+            county = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.COUNTY
+            ].mode()
             county = county.values[0]
 
         return county
 
     @property
     def elevation(self):
         """Get the SC point elevation based on the resource meta data."""
         elevation = None
-        if 'elevation' in self.h5.meta:
-            elevation = self.h5.meta.loc[self.h5_gid_set, 'elevation'].mean()
+        if ResourceMetaField.ELEVATION in self.h5.meta:
+            elevation = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.ELEVATION
+            ].mean()
 
         return elevation
 
     @property
     def timezone(self):
         """Get the SC point timezone based on the resource meta data."""
         timezone = None
-        if 'timezone' in self.h5.meta and self.county is not None:
+        county_not_none = self.county is not None
+        if ResourceMetaField.TIMEZONE in self.h5.meta and county_not_none:
             # make sure timezone flag and county are coincident
-            counties = self.h5.meta.loc[self.h5_gid_set, 'county'].values
+            counties = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.COUNTY
+            ].values
             iloc = np.where(counties == self.county)[0][0]
-            timezone = self.h5.meta.loc[self.h5_gid_set, 'timezone'].values
+            timezone = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.TIMEZONE
+            ].values
             timezone = timezone[iloc]
 
-        elif 'timezone' in self.h5.meta:
-            timezone = self.h5.meta.loc[self.h5_gid_set, 'timezone'].mode()
+        elif ResourceMetaField.TIMEZONE in self.h5.meta:
+            timezone = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.TIMEZONE
+            ].mode()
             timezone = timezone.values[0]
 
         return timezone
 
     @property
     def offshore(self):
         """Get the SC point offshore flag based on the resource meta data
         (if offshore column is present)."""
         offshore = None
-        if 'offshore' in self.h5.meta and self.county is not None:
+        county_not_none = self.county is not None
+        if ResourceMetaField.OFFSHORE in self.h5.meta and county_not_none:
             # make sure offshore flag and county are coincident
-            counties = self.h5.meta.loc[self.h5_gid_set, 'county'].values
+            counties = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.COUNTY
+            ].values
             iloc = np.where(counties == self.county)[0][0]
-            offshore = self.h5.meta.loc[self.h5_gid_set, 'offshore'].values
+            offshore = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.OFFSHORE
+            ].values
             offshore = offshore[iloc]
 
-        elif 'offshore' in self.h5.meta:
-            offshore = self.h5.meta.loc[self.h5_gid_set, 'offshore'].mode()
+        elif ResourceMetaField.OFFSHORE in self.h5.meta:
+            offshore = self.h5.meta.loc[
+                self.h5_gid_set, ResourceMetaField.OFFSHORE
+            ].mode()
             offshore = offshore.values[0]
 
         return offshore
 
     @property
     def gid_counts(self):
         """Get the sum of the inclusion values in each resource/generation gid
@@ -1134,51 +1250,66 @@
         than the value provided by n_gids if fractional exclusion/inclusions
         are provided.
 
         Returns
         -------
         gid_counts : list
         """
-        gid_counts = [self.include_mask_flat[(self._h5_gids == gid)].sum()
-                      for gid in self.h5_gid_set]
+        gid_counts = [
+            self.include_mask_flat[(self._h5_gids == gid)].sum()
+            for gid in self.h5_gid_set
+        ]
 
         return gid_counts
 
     @property
     def summary(self):
         """
         Supply curve point's meta data summary
 
         Returns
         -------
         pandas.Series
             List of supply curve point's meta data
         """
-        meta = {'sc_point_gid': self.sc_point_gid,
-                'source_gids': self.h5_gid_set,
-                'gid_counts': self.gid_counts,
-                'n_gids': self.n_gids,
-                'area_sq_km': self.area,
-                'latitude': self.latitude,
-                'longitude': self.longitude,
-                'country': self.country,
-                'state': self.state,
-                'county': self.county,
-                'elevation': self.elevation,
-                'timezone': self.timezone,
-                }
+        meta = {
+            SupplyCurveField.SC_POINT_GID: self.sc_point_gid,
+            SupplyCurveField.SOURCE_GIDS: self.h5_gid_set,
+            SupplyCurveField.GID_COUNTS: self.gid_counts,
+            SupplyCurveField.N_GIDS: self.n_gids,
+            SupplyCurveField.AREA_SQ_KM: self.area,
+            SupplyCurveField.LATITUDE: self.latitude,
+            SupplyCurveField.LONGITUDE: self.longitude,
+            SupplyCurveField.COUNTRY: self.country,
+            SupplyCurveField.STATE: self.state,
+            SupplyCurveField.COUNTY: self.county,
+            SupplyCurveField.ELEVATION: self.elevation,
+            SupplyCurveField.TIMEZONE: self.timezone,
+        }
         meta = pd.Series(meta)
 
         return meta
 
     @classmethod
-    def run(cls, gid, excl, agg_h5, tm_dset, *agg_dset, agg_method='mean',
-            excl_dict=None, inclusion_mask=None,
-            resolution=64, excl_area=None,
-            exclusion_shape=None, close=True, gen_index=None):
+    def run(
+        cls,
+        gid,
+        excl,
+        agg_h5,
+        tm_dset,
+        *agg_dset,
+        agg_method="mean",
+        excl_dict=None,
+        inclusion_mask=None,
+        resolution=64,
+        excl_area=None,
+        exclusion_shape=None,
+        close=True,
+        gen_index=None,
+    ):
         """
         Compute exclusions weight mean for the sc point from data
 
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
@@ -1224,60 +1355,80 @@
 
         Returns
         -------
         out : dict
             Given datasets and meta data aggregated to supply curve points
         """
         if isinstance(agg_dset, str):
-            agg_dset = (agg_dset, )
+            agg_dset = (agg_dset,)
 
-        kwargs = {"excl_dict": excl_dict,
-                  "inclusion_mask": inclusion_mask,
-                  "resolution": resolution,
-                  "excl_area": excl_area,
-                  "exclusion_shape": exclusion_shape,
-                  "close": close,
-                  "gen_index": gen_index}
+        kwargs = {
+            "excl_dict": excl_dict,
+            "inclusion_mask": inclusion_mask,
+            "resolution": resolution,
+            "excl_area": excl_area,
+            "exclusion_shape": exclusion_shape,
+            "close": close,
+            "gen_index": gen_index,
+        }
 
         with cls(gid, excl, agg_h5, tm_dset, **kwargs) as point:
-            if agg_method.lower().startswith('mean'):
+            if agg_method.lower().startswith("mean"):
                 agg_method = point.exclusion_weighted_mean
-            elif agg_method.lower().startswith(('sum', 'agg')):
+            elif agg_method.lower().startswith(("sum", "agg")):
                 agg_method = point.aggregate
-            elif 'wind_dir' in agg_method.lower():
+            elif "wind_dir" in agg_method.lower():
                 agg_method = point.mean_wind_dirs
             else:
-                msg = ('Aggregation method must be either mean, '
-                       'sum/aggregate, or wind_dir')
+                msg = (
+                    "Aggregation method must be either mean, "
+                    "sum/aggregate, or wind_dir"
+                )
                 logger.error(msg)
                 raise ValueError(msg)
 
-            out = {'meta': point.summary}
+            out = {"meta": point.summary}
 
             for dset in agg_dset:
                 ds = point.h5.open_dataset(dset)
                 out[dset] = agg_method(ds)
 
         return out
 
 
 class GenerationSupplyCurvePoint(AggregationSupplyCurvePoint):
     """Supply curve point summary framework that ties a reV SC point to its
     respective generation and resource data."""
 
     # technology-dependent power density estimates in MW/km2
-    POWER_DENSITY = {'pv': 36, 'wind': 3}
+    POWER_DENSITY = {"pv": 36, "wind": 3}
 
-    def __init__(self, gid, excl, gen, tm_dset, gen_index,
-                 excl_dict=None, inclusion_mask=None,
-                 res_class_dset=None, res_class_bin=None, excl_area=None,
-                 power_density=None, cf_dset='cf_mean-means',
-                 lcoe_dset='lcoe_fcr-means', h5_dsets=None, resolution=64,
-                 exclusion_shape=None, close=False, friction_layer=None,
-                 recalc_lcoe=True, apply_exclusions=True):
+    def __init__(
+        self,
+        gid,
+        excl,
+        gen,
+        tm_dset,
+        gen_index,
+        excl_dict=None,
+        inclusion_mask=None,
+        res_class_dset=None,
+        res_class_bin=None,
+        excl_area=None,
+        power_density=None,
+        cf_dset="cf_mean-means",
+        lcoe_dset="lcoe_fcr-means",
+        h5_dsets=None,
+        resolution=64,
+        exclusion_shape=None,
+        close=False,
+        friction_layer=None,
+        recalc_lcoe=True,
+        apply_exclusions=True,
+    ):
         """
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
         excl : str | ExclusionMask
             Filepath to exclusions h5 or ExclusionMask file handler.
@@ -1356,34 +1507,44 @@
         self._gen_data = None
         self._lcoe_data = None
         self._pd_obj = None
         self._power_density = self._power_density_ac = power_density
         self._friction_layer = friction_layer
         self._recalc_lcoe = recalc_lcoe
 
-        super().__init__(gid, excl, gen, tm_dset,
-                         excl_dict=excl_dict,
-                         inclusion_mask=inclusion_mask,
-                         resolution=resolution,
-                         excl_area=excl_area,
-                         exclusion_shape=exclusion_shape,
-                         close=close, apply_exclusions=False)
+        super().__init__(
+            gid,
+            excl,
+            gen,
+            tm_dset,
+            excl_dict=excl_dict,
+            inclusion_mask=inclusion_mask,
+            resolution=resolution,
+            excl_area=excl_area,
+            exclusion_shape=exclusion_shape,
+            close=close,
+            apply_exclusions=False,
+        )
 
         self._res_gid_set = None
         self._gen_gid_set = None
 
         self._gen_fpath, self._gen = self._h5_fpath, self._h5
 
-        self._gen_gids, self._res_gids = self._map_gen_gids(self._gids,
-                                                            gen_index)
+        self._gen_gids, self._res_gids = self._map_gen_gids(
+            self._gids, gen_index
+        )
         self._gids = self._gen_gids
         if (self._gen_gids != -1).sum() == 0:
-            emsg = ('Supply curve point gid {} has no viable exclusion '
-                    'points based on exclusions file: "{}"'
-                    .format(self._gid, self._excl_fpath))
+            emsg = (
+                "Supply curve point gid {} has no viable exclusion "
+                'points based on exclusions file: "{}"'.format(
+                    self._gid, self._excl_fpath
+                )
+            )
             raise EmptySupplyCurvePointError(emsg)
 
         if apply_exclusions:
             self._apply_exclusions()
 
     def exclusion_weighted_mean(self, flat_arr):
         """Calc the exclusions-weighted mean value of a flat array of gen data.
@@ -1397,15 +1558,15 @@
 
         Returns
         -------
         mean : float
             Mean of flat_arr masked by the binary exclusions then weighted by
             the non-zero exclusions.
         """
-        x = flat_arr[self._gen_gids[self.bool_mask]].astype('float32')
+        x = flat_arr[self._gen_gids[self.bool_mask]].astype("float32")
         incl = self.include_mask_flat[self.bool_mask]
         x *= incl
         mean = x.sum() / incl.sum()
 
         return mean
 
     @property
@@ -1472,16 +1633,18 @@
         corresponding to this sc point.
 
         Returns
         -------
         gid_counts : list
             List of exclusion pixels in each resource/generation gid.
         """
-        gid_counts = [self.include_mask_flat[(self._res_gids == gid)].sum()
-                      for gid in self.res_gid_set]
+        gid_counts = [
+            self.include_mask_flat[(self._res_gids == gid)].sum()
+            for gid in self.res_gid_set
+        ]
 
         return gid_counts
 
     @property
     def res_data(self):
         """Get the resource data array.
 
@@ -1491,18 +1654,17 @@
             Multi-year-mean resource data array for all sites in the
             generation data output file.
         """
 
         if isinstance(self._res_class_dset, np.ndarray):
             return self._res_class_dset
 
-        else:
-            if self._res_data is None:
-                if self._res_class_dset in self.gen.datasets:
-                    self._res_data = self.gen[self._res_class_dset]
+        if self._res_data is None:
+            if self._res_class_dset in self.gen.datasets:
+                self._res_data = self.gen[self._res_class_dset]
 
         return self._res_data
 
     @property
     def gen_data(self):
         """Get the generation capacity factor data array.
 
@@ -1512,18 +1674,17 @@
             Multi-year-mean capacity factor data array for all sites in the
             generation data output file.
         """
 
         if isinstance(self._cf_dset, np.ndarray):
             return self._cf_dset
 
-        else:
-            if self._gen_data is None:
-                if self._cf_dset in self.gen.datasets:
-                    self._gen_data = self.gen[self._cf_dset]
+        if self._gen_data is None:
+            if self._cf_dset in self.gen.datasets:
+                self._gen_data = self.gen[self._cf_dset]
 
         return self._gen_data
 
     @property
     def lcoe_data(self):
         """Get the LCOE data array.
 
@@ -1533,18 +1694,17 @@
             Multi-year-mean LCOE data array for all sites in the
             generation data output file.
         """
 
         if isinstance(self._lcoe_dset, np.ndarray):
             return self._lcoe_dset
 
-        else:
-            if self._lcoe_data is None:
-                if self._lcoe_dset in self.gen.datasets:
-                    self._lcoe_data = self.gen[self._lcoe_dset]
+        if self._lcoe_data is None:
+            if self._lcoe_dset in self.gen.datasets:
+                self._lcoe_data = self.gen[self._lcoe_dset]
 
         return self._lcoe_data
 
     @property
     def mean_cf(self):
         """Get the mean capacity factor for the non-excluded data. Capacity
         factor is weighted by the exclusions (usually 0 or 1, but 0.5
@@ -1574,30 +1734,39 @@
         mean_lcoe = None
 
         # prioritize the calculation of lcoe explicitly from the multi year
         # mean CF (the lcoe re-calc will still happen if mean_cf is a single
         # year CF, but the output should be identical to the original LCOE and
         # so is not consequential).
         if self._recalc_lcoe:
-            required = ('fixed_charge_rate', 'capital_cost',
-                        'fixed_operating_cost', 'variable_operating_cost',
-                        'system_capacity')
-            if self.mean_h5_dsets_data is not None:
-                if all(k in self.mean_h5_dsets_data for k in required):
-                    aep = (self.mean_h5_dsets_data['system_capacity']
-                           * self.mean_cf * 8760)
-                    # Note the AEP computation uses the SAM config
-                    # `system_capacity`, so no need to scale `capital_cost`
-                    # or `fixed_operating_cost` by anything
-                    mean_lcoe = lcoe_fcr(
-                        self.mean_h5_dsets_data['fixed_charge_rate'],
-                        self.mean_h5_dsets_data['capital_cost'],
-                        self.mean_h5_dsets_data['fixed_operating_cost'],
-                        aep,
-                        self.mean_h5_dsets_data['variable_operating_cost'])
+            required = (
+                "fixed_charge_rate",
+                "capital_cost",
+                "fixed_operating_cost",
+                "variable_operating_cost",
+                "system_capacity",
+            )
+            if self.mean_h5_dsets_data is not None and all(
+                k in self.mean_h5_dsets_data for k in required
+            ):
+                aep = (
+                    self.mean_h5_dsets_data["system_capacity"]
+                    * self.mean_cf
+                    * 8760
+                )
+                # Note the AEP computation uses the SAM config
+                # `system_capacity`, so no need to scale `capital_cost`
+                # or `fixed_operating_cost` by anything
+                mean_lcoe = lcoe_fcr(
+                    self.mean_h5_dsets_data["fixed_charge_rate"],
+                    self.mean_h5_dsets_data["capital_cost"],
+                    self.mean_h5_dsets_data["fixed_operating_cost"],
+                    aep,
+                    self.mean_h5_dsets_data["variable_operating_cost"],
+                )
 
         # alternative if lcoe was not able to be re-calculated from
         # multi year mean CF
         if mean_lcoe is None and self.lcoe_data is not None:
             mean_lcoe = self.exclusion_weighted_mean(self.lcoe_data)
 
         return mean_lcoe
@@ -1675,34 +1844,39 @@
         Returns
         -------
         _power_density : float
             Estimated power density in MW/km2
         """
 
         if self._power_density is None:
-            tech = self.gen.meta['reV_tech'][0]
+            tech = self.gen.meta["reV_tech"][0]
             if tech in self.POWER_DENSITY:
                 self._power_density = self.POWER_DENSITY[tech]
             else:
-                warn('Could not recognize reV technology in generation meta '
-                     'data: "{}". Cannot lookup an appropriate power density '
-                     'to calculate SC point capacity.'.format(tech))
+                warn(
+                    "Could not recognize reV technology in generation meta "
+                    'data: "{}". Cannot lookup an appropriate power density '
+                    "to calculate SC point capacity.".format(tech)
+                )
 
         elif isinstance(self._power_density, pd.DataFrame):
             self._pd_obj = self._power_density
 
             missing = set(self.res_gid_set) - set(self._pd_obj.index.values)
             if any(missing):
-                msg = ('Variable power density input is missing the '
-                       'following resource GIDs: {}'.format(missing))
+                msg = (
+                    "Variable power density input is missing the "
+                    "following resource GIDs: {}".format(missing)
+                )
                 logger.error(msg)
                 raise FileInputError(msg)
 
-            pds = self._pd_obj.loc[self._res_gids[self.bool_mask],
-                                   'power_density'].values
+            pds = self._pd_obj.loc[
+                self._res_gids[self.bool_mask], "power_density"
+            ].values
             pds = pds.astype(np.float32)
             pds *= self.include_mask_flat[self.bool_mask]
             denom = self.include_mask_flat[self.bool_mask].sum()
             self._power_density = pds.sum() / denom
 
         return self._power_density
 
@@ -1720,40 +1894,45 @@
         _power_density_ac : float | None
             Estimated AC power density in MW/km2
         """
         if "dc_ac_ratio" not in self.gen.datasets:
             return None
 
         ilr = self.gen["dc_ac_ratio", self._gen_gids[self.bool_mask]]
-        ilr = ilr.astype('float32')
+        ilr = ilr.astype("float32")
         weights = self.include_mask_flat[self.bool_mask]
         if self._power_density_ac is None:
-            tech = self.gen.meta['reV_tech'][0]
+            tech = self.gen.meta["reV_tech"][0]
             if tech in self.POWER_DENSITY:
                 power_density_ac = self.POWER_DENSITY[tech] / ilr
                 power_density_ac *= weights
                 power_density_ac = power_density_ac.sum() / weights.sum()
             else:
-                warn('Could not recognize reV technology in generation meta '
-                     'data: "{}". Cannot lookup an appropriate power density '
-                     'to calculate SC point capacity.'.format(tech))
+                warn(
+                    "Could not recognize reV technology in generation meta "
+                    'data: "{}". Cannot lookup an appropriate power density '
+                    "to calculate SC point capacity.".format(tech)
+                )
                 power_density_ac = None
 
         elif isinstance(self._power_density_ac, pd.DataFrame):
             self._pd_obj = self._power_density_ac
 
             missing = set(self.res_gid_set) - set(self._pd_obj.index.values)
             if any(missing):
-                msg = ('Variable power density input is missing the '
-                       'following resource GIDs: {}'.format(missing))
+                msg = (
+                    "Variable power density input is missing the "
+                    "following resource GIDs: {}".format(missing)
+                )
                 logger.error(msg)
                 raise FileInputError(msg)
 
-            pds = self._pd_obj.loc[self._res_gids[self.bool_mask],
-                                   'power_density'].values
+            pds = self._pd_obj.loc[
+                self._res_gids[self.bool_mask], "power_density"
+            ].values
             power_density_ac = pds.astype(np.float32) / ilr
             power_density_ac *= weights
             power_density_ac = power_density_ac.sum() / weights.sum()
         else:
             power_density_ac = self._power_density_ac * weights / ilr
             power_density_ac = power_density_ac.sum() / weights.sum()
 
@@ -1812,20 +1991,22 @@
         -------
         sc_point_capital_cost : float | None
             Total supply curve point capital cost ($).
         """
         if self.mean_h5_dsets_data is None:
             return None
 
-        required = ('capital_cost', 'system_capacity')
+        required = ("capital_cost", "system_capacity")
         if not all(k in self.mean_h5_dsets_data for k in required):
             return None
 
-        cap_cost_per_mw = (self.mean_h5_dsets_data['capital_cost']
-                           / self.mean_h5_dsets_data['system_capacity'])
+        cap_cost_per_mw = (
+            self.mean_h5_dsets_data["capital_cost"]
+            / self.mean_h5_dsets_data["system_capacity"]
+        )
         return cap_cost_per_mw * self.capacity
 
     @property
     def sc_point_fixed_operating_cost(self):
         """Get the fixed operating cost for the entire SC point.
 
         This method scales the fixed operating cost based on the
@@ -1838,20 +2019,22 @@
         -------
         sc_point_fixed_operating_cost : float | None
             Total supply curve point fixed operating cost ($).
         """
         if self.mean_h5_dsets_data is None:
             return None
 
-        required = ('fixed_operating_cost', 'system_capacity')
+        required = ("fixed_operating_cost", "system_capacity")
         if not all(k in self.mean_h5_dsets_data for k in required):
             return None
 
-        fixed_cost_per_mw = (self.mean_h5_dsets_data['fixed_operating_cost']
-                             / self.mean_h5_dsets_data['system_capacity'])
+        fixed_cost_per_mw = (
+            self.mean_h5_dsets_data["fixed_operating_cost"]
+            / self.mean_h5_dsets_data["system_capacity"]
+        )
         return fixed_cost_per_mw * self.capacity
 
     @property
     def sc_point_annual_energy(self):
         """Get the total annual energy (MWh) for the entire SC point.
 
         This value is computed using the capacity of the supply curve
@@ -1905,18 +2088,21 @@
                 if dset in self.gen.datasets:
                     _h5_dsets_data[dset] = self.gen[dset]
 
         elif isinstance(self._h5_dsets, dict):
             _h5_dsets_data = self._h5_dsets
 
         elif self._h5_dsets is not None:
-            e = ('Cannot recognize h5_dsets input type, should be None, '
-                 'a list of dataset names, or a dictionary or '
-                 'pre-extracted data. Received: {} {}'
-                 .format(type(self._h5_dsets), self._h5_dsets))
+            e = (
+                "Cannot recognize h5_dsets input type, should be None, "
+                "a list of dataset names, or a dictionary or "
+                "pre-extracted data. Received: {} {}".format(
+                    type(self._h5_dsets), self._h5_dsets
+                )
+            )
             logger.error(e)
             raise TypeError(e)
 
         return _h5_dsets_data
 
     @property
     def mean_h5_dsets_data(self):
@@ -1951,16 +2137,18 @@
         # ensure that excluded pixels (including resource exclusions!)
         # has an exclusions multiplier of 0
         exclude = exclude.reshape(self.include_mask.shape)
         self._incl_mask[exclude] = 0.0
         self._incl_mask = self._incl_mask.flatten()
 
         if (self._gen_gids != -1).sum() == 0:
-            msg = ('Supply curve point gid {} is completely excluded for res '
-                   'bin: {}'.format(self._gid, self._res_class_bin))
+            msg = (
+                "Supply curve point gid {} is completely excluded for res "
+                "bin: {}".format(self._gid, self._res_class_bin)
+            )
             raise EmptySupplyCurvePointError(msg)
 
     def _resource_exclusion(self, boolean_exclude):
         """Include the resource exclusion into a pre-existing bool exclusion.
 
         Parameters
         ----------
@@ -1970,22 +2158,24 @@
         Returns
         -------
         boolean_exclude : np.ndarray
             Same as input but includes additional exclusions for resource
             outside of current resource class bin.
         """
 
-        if (self._res_class_dset is not None
-                and self._res_class_bin is not None):
-
+        if (
+            self._res_class_dset is not None
+            and self._res_class_bin is not None
+        ):
             rex = self.res_data[self._gen_gids]
-            rex = ((rex < np.min(self._res_class_bin))
-                   | (rex >= np.max(self._res_class_bin)))
+            rex = (rex < np.min(self._res_class_bin)) | (
+                rex >= np.max(self._res_class_bin)
+            )
 
-            boolean_exclude = (boolean_exclude | rex)
+            boolean_exclude = boolean_exclude | rex
 
         return boolean_exclude
 
     def point_summary(self, args=None):
         """
         Get a summary dictionary of a single supply curve point.
 
@@ -1997,58 +2187,72 @@
 
         Returns
         -------
         summary : dict
             Dictionary of summary outputs for this sc point.
         """
 
-        ARGS = {'res_gids': self.res_gid_set,
-                'gen_gids': self.gen_gid_set,
-                'gid_counts': self.gid_counts,
-                'n_gids': self.n_gids,
-                'mean_cf': self.mean_cf,
-                'mean_lcoe': self.mean_lcoe,
-                'mean_res': self.mean_res,
-                'capacity': self.capacity,
-                'area_sq_km': self.area,
-                'latitude': self.latitude,
-                'longitude': self.longitude,
-                'country': self.country,
-                'state': self.state,
-                'county': self.county,
-                'elevation': self.elevation,
-                'timezone': self.timezone,
-                }
-
-        extra_atts = ['capacity_ac', 'offshore', 'sc_point_capital_cost',
-                      'sc_point_fixed_operating_cost',
-                      'sc_point_annual_energy', 'sc_point_annual_energy_ac']
-        for attr in extra_atts:
-            value = getattr(self, attr)
+        ARGS = {
+            SupplyCurveField.LATITUDE: self.latitude,
+            SupplyCurveField.LONGITUDE: self.longitude,
+            SupplyCurveField.TIMEZONE: self.timezone,
+            SupplyCurveField.COUNTRY: self.country,
+            SupplyCurveField.STATE: self.state,
+            SupplyCurveField.COUNTY: self.county,
+            SupplyCurveField.ELEVATION: self.elevation,
+            SupplyCurveField.RES_GIDS: self.res_gid_set,
+            SupplyCurveField.GEN_GIDS: self.gen_gid_set,
+            SupplyCurveField.GID_COUNTS: self.gid_counts,
+            SupplyCurveField.N_GIDS: self.n_gids,
+            SupplyCurveField.MEAN_CF: self.mean_cf,
+            SupplyCurveField.MEAN_LCOE: self.mean_lcoe,
+            SupplyCurveField.MEAN_RES: self.mean_res,
+            SupplyCurveField.CAPACITY: self.capacity,
+            SupplyCurveField.AREA_SQ_KM: self.area,
+        }
+
+        extra_atts = {
+            SupplyCurveField.CAPACITY_AC: self.capacity_ac,
+            SupplyCurveField.OFFSHORE: self.offshore,
+            SupplyCurveField.SC_POINT_CAPITAL_COST: self.sc_point_capital_cost,
+            SupplyCurveField.SC_POINT_FIXED_OPERATING_COST: (
+                self.sc_point_fixed_operating_cost
+            ),
+            SupplyCurveField.SC_POINT_ANNUAL_ENERGY: (
+                self.sc_point_annual_energy
+            ),
+            SupplyCurveField.SC_POINT_ANNUAL_ENERGY_AC: (
+                self.sc_point_annual_energy_ac
+            ),
+        }
+        for attr, value in extra_atts.items():
             if value is not None:
                 ARGS[attr] = value
 
         if self._friction_layer is not None:
-            ARGS['mean_friction'] = self.mean_friction
-            ARGS['mean_lcoe_friction'] = self.mean_lcoe_friction
+            ARGS[SupplyCurveField.MEAN_FRICTION] = self.mean_friction
+            ARGS[SupplyCurveField.MEAN_LCOE_FRICTION] = self.mean_lcoe_friction
 
         if self._h5_dsets is not None:
             for dset, data in self.mean_h5_dsets_data.items():
-                ARGS['mean_{}'.format(dset)] = data
+                ARGS["mean_{}".format(dset)] = data
 
         if args is None:
             args = list(ARGS.keys())
 
         summary = {}
         for arg in args:
             if arg in ARGS:
                 summary[arg] = ARGS[arg]
             else:
-                warn('Cannot find "{}" as an available SC self summary '
-                     'output', OutputWarning)
+                warn(
+                    'Cannot find "{}" as an available SC self summary '
+                    "output",
+                    OutputWarning,
+                )
 
         return summary
 
     @staticmethod
     def economies_of_scale(cap_cost_scale, summary):
         """Apply economies of scale to this point summary
 
@@ -2066,34 +2270,55 @@
         Returns
         -------
         summary : dict
             Dictionary of summary outputs for this sc point.
         """
 
         eos = EconomiesOfScale(cap_cost_scale, summary)
-        summary['raw_lcoe'] = eos.raw_lcoe
-        summary['mean_lcoe'] = eos.scaled_lcoe
-        summary['capital_cost_scalar'] = eos.capital_cost_scalar
-        summary['scaled_capital_cost'] = eos.scaled_capital_cost
-        if "sc_point_capital_cost" in summary:
-            scaled_costs = (summary["sc_point_capital_cost"]
-                            * eos.capital_cost_scalar)
-            summary['scaled_sc_point_capital_cost'] = scaled_costs
+        summary[SupplyCurveField.RAW_LCOE] = eos.raw_lcoe
+        summary[SupplyCurveField.MEAN_LCOE] = eos.scaled_lcoe
+        summary[SupplyCurveField.CAPITAL_COST_SCALAR] = eos.capital_cost_scalar
+        summary[SupplyCurveField.SCALED_CAPITAL_COST] = eos.scaled_capital_cost
+        if SupplyCurveField.SC_POINT_CAPITAL_COST in summary:
+            scaled_costs = (
+                summary[SupplyCurveField.SC_POINT_CAPITAL_COST]
+                * eos.capital_cost_scalar
+            )
+            summary[SupplyCurveField.SCALED_SC_POINT_CAPITAL_COST] = (
+                scaled_costs
+            )
 
         return summary
 
     @classmethod
-    def summarize(cls, gid, excl_fpath, gen_fpath, tm_dset, gen_index,
-                  excl_dict=None, inclusion_mask=None,
-                  res_class_dset=None, res_class_bin=None,
-                  excl_area=None, power_density=None,
-                  cf_dset='cf_mean-means', lcoe_dset='lcoe_fcr-means',
-                  h5_dsets=None, resolution=64, exclusion_shape=None,
-                  close=False, friction_layer=None, args=None,
-                  data_layers=None, cap_cost_scale=None, recalc_lcoe=True):
+    def summarize(
+        cls,
+        gid,
+        excl_fpath,
+        gen_fpath,
+        tm_dset,
+        gen_index,
+        excl_dict=None,
+        inclusion_mask=None,
+        res_class_dset=None,
+        res_class_bin=None,
+        excl_area=None,
+        power_density=None,
+        cf_dset="cf_mean-means",
+        lcoe_dset="lcoe_fcr-means",
+        h5_dsets=None,
+        resolution=64,
+        exclusion_shape=None,
+        close=False,
+        friction_layer=None,
+        args=None,
+        data_layers=None,
+        cap_cost_scale=None,
+        recalc_lcoe=True,
+    ):
         """Get a summary dictionary of a single supply curve point.
 
         Parameters
         ----------
         gid : int
             gid for supply curve point to analyze.
         excl_fpath : str
@@ -2172,32 +2397,34 @@
             and variable_operating_cost.
 
         Returns
         -------
         summary : dict
             Dictionary of summary outputs for this sc point.
         """
-        kwargs = {"excl_dict": excl_dict,
-                  "inclusion_mask": inclusion_mask,
-                  "res_class_dset": res_class_dset,
-                  "res_class_bin": res_class_bin,
-                  "excl_area": excl_area,
-                  "power_density": power_density,
-                  "cf_dset": cf_dset,
-                  "lcoe_dset": lcoe_dset,
-                  "h5_dsets": h5_dsets,
-                  "resolution": resolution,
-                  "exclusion_shape": exclusion_shape,
-                  "close": close,
-                  'friction_layer': friction_layer,
-                  'recalc_lcoe': recalc_lcoe,
-                  }
-
-        with cls(gid, excl_fpath, gen_fpath, tm_dset, gen_index,
-                 **kwargs) as point:
+        kwargs = {
+            "excl_dict": excl_dict,
+            "inclusion_mask": inclusion_mask,
+            "res_class_dset": res_class_dset,
+            "res_class_bin": res_class_bin,
+            "excl_area": excl_area,
+            "power_density": power_density,
+            "cf_dset": cf_dset,
+            "lcoe_dset": lcoe_dset,
+            "h5_dsets": h5_dsets,
+            "resolution": resolution,
+            "exclusion_shape": exclusion_shape,
+            "close": close,
+            "friction_layer": friction_layer,
+            "recalc_lcoe": recalc_lcoe,
+        }
+
+        with cls(
+            gid, excl_fpath, gen_fpath, tm_dset, gen_index, **kwargs
+        ) as point:
             summary = point.point_summary(args=args)
 
             if data_layers is not None:
                 summary = point.agg_data_layers(summary, data_layers)
 
             if cap_cost_scale is not None:
                 summary = point.economies_of_scale(cap_cost_scale, summary)
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/sc_aggregation.py` & `NREL-reV-0.8.9/reV/supply_curve/sc_aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,55 +2,70 @@
 # pylint: disable=anomalous-backslash-in-string
 """reV supply curve aggregation framework.
 
 Created on Fri Jun 21 13:24:31 2019
 
 @author: gbuster
 """
-from concurrent.futures import as_completed
 import logging
-import numpy as np
-import psutil
 import os
-import pandas as pd
+from concurrent.futures import as_completed
 from warnings import warn
 
+import numpy as np
+import pandas as pd
+import psutil
+from rex.multi_file_resource import MultiFileResource
+from rex.resource import Resource
+from rex.utilities.execution import SpawnProcessPool
+
 from reV.generation.base import BaseGen
 from reV.handlers.exclusions import ExclusionLayers
-from reV.supply_curve.aggregation import (AbstractAggFileHandler,
-                                          BaseAggregation, Aggregation)
+from reV.supply_curve.aggregation import (
+    AbstractAggFileHandler,
+    Aggregation,
+    BaseAggregation,
+)
 from reV.supply_curve.exclusions import FrictionMask
 from reV.supply_curve.extent import SupplyCurveExtent
 from reV.supply_curve.points import GenerationSupplyCurvePoint
-from reV.utilities.exceptions import (EmptySupplyCurvePointError,
-                                      OutputWarning, FileInputError,
-                                      InputWarning)
-from reV.utilities import log_versions
-
-from rex.resource import Resource
-from rex.multi_file_resource import MultiFileResource
-from rex.utilities.execution import SpawnProcessPool
+from reV.utilities import SupplyCurveField, log_versions
+from reV.utilities.exceptions import (
+    EmptySupplyCurvePointError,
+    FileInputError,
+    InputWarning,
+    OutputWarning,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class SupplyCurveAggFileHandler(AbstractAggFileHandler):
     """
     Framework to handle aggregation summary context managers:
     - exclusions .h5 file
     - generation .h5 file
     - econ .h5 file (optional)
     - friction surface .h5 file (optional)
     - variable power density .csv (optional)
     """
 
-    def __init__(self, excl_fpath, gen_fpath, econ_fpath=None,
-                 data_layers=None, power_density=None, excl_dict=None,
-                 friction_fpath=None, friction_dset=None,
-                 area_filter_kernel='queen', min_area=None):
+    def __init__(
+        self,
+        excl_fpath,
+        gen_fpath,
+        econ_fpath=None,
+        data_layers=None,
+        power_density=None,
+        excl_dict=None,
+        friction_fpath=None,
+        friction_dset=None,
+        area_filter_kernel="queen",
+        min_area=None,
+    ):
         """
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
             (can be one or more filepaths).
         gen_fpath : str
@@ -85,32 +100,35 @@
             Must be paired with friction_fpath. Must be same shape as
             exclusions.
         area_filter_kernel : str
             Contiguous area filter method to use on final exclusions mask
         min_area : float | None
             Minimum required contiguous area filter in sq-km
         """
-        super().__init__(excl_fpath, excl_dict=excl_dict,
-                         area_filter_kernel=area_filter_kernel,
-                         min_area=min_area)
+        super().__init__(
+            excl_fpath,
+            excl_dict=excl_dict,
+            area_filter_kernel=area_filter_kernel,
+            min_area=min_area,
+        )
 
         self._gen = self._open_gen_econ_resource(gen_fpath, econ_fpath)
         # pre-initialize the resource meta data
         _ = self._gen.meta
 
         self._data_layers = data_layers
         self._power_density = power_density
         self._parse_power_density()
 
         self._friction_layer = None
         if friction_fpath is not None and friction_dset is not None:
             self._friction_layer = FrictionMask(friction_fpath, friction_dset)
 
             if not np.all(self._friction_layer.shape == self._excl.shape):
-                e = ('Friction layer shape {} must match exclusions shape {}!'
+                e = ("Friction layer shape {} must match exclusions shape {}!"
                      .format(self._friction_layer.shape, self._excl.shape))
                 logger.error(e)
                 raise FileInputError(e)
 
     @staticmethod
     def _open_gen_econ_resource(gen_fpath, econ_fpath):
         """Open a rex resource file handler for the reV generation and
@@ -128,45 +146,50 @@
         -------
         handler : Resource | MultiFileResource
             Open resource handler initialized with gen_fpath and (optionally)
             econ_fpath.
         """
 
         handler = None
-        is_gen_h5 = isinstance(gen_fpath, str) and gen_fpath.endswith('.h5')
-        is_econ_h5 = isinstance(econ_fpath, str) and econ_fpath.endswith('.h5')
+        is_gen_h5 = isinstance(gen_fpath, str) and gen_fpath.endswith(".h5")
+        is_econ_h5 = isinstance(econ_fpath, str) and econ_fpath.endswith(".h5")
 
         if is_gen_h5 and not is_econ_h5:
             handler = Resource(gen_fpath)
         elif is_gen_h5 and is_econ_h5:
-            handler = MultiFileResource([gen_fpath, econ_fpath],
-                                        check_files=True)
+            handler = MultiFileResource(
+                [gen_fpath, econ_fpath], check_files=True
+            )
 
         return handler
 
     def _parse_power_density(self):
         """Parse the power density input. If file, open file handler."""
 
         if isinstance(self._power_density, str):
             self._pdf = self._power_density
 
-            if self._pdf.endswith('.csv'):
+            if self._pdf.endswith(".csv"):
                 self._power_density = pd.read_csv(self._pdf)
-                if ('gid' in self._power_density
+                if (SupplyCurveField.GID in self._power_density
                         and 'power_density' in self._power_density):
-                    self._power_density = self._power_density.set_index('gid')
+                    self._power_density = \
+                        self._power_density.set_index(SupplyCurveField.GID)
                 else:
-                    msg = ('Variable power density file must include "gid" '
+                    msg = ('Variable power density file must include "{}" '
                            'and "power_density" columns, but received: {}'
-                           .format(self._power_density.columns.values))
+                           .format(SupplyCurveField.GID,
+                                   self._power_density.columns.values))
                     logger.error(msg)
                     raise FileInputError(msg)
             else:
-                msg = ('Variable power density file must be csv but received: '
-                       '{}'.format(self._pdf))
+                msg = (
+                    "Variable power density file must be csv but received: "
+                    "{}".format(self._pdf)
+                )
                 logger.error(msg)
                 raise FileInputError(msg)
 
     def close(self):
         """Close all file handlers."""
         self._excl.close()
         self._gen.close()
@@ -227,15 +250,15 @@
                  excl_dict=None, area_filter_kernel='queen', min_area=None,
                  resolution=64, excl_area=None, res_fpath=None, gids=None,
                  pre_extract_inclusions=False, res_class_dset=None,
                  res_class_bins=None, cf_dset='cf_mean-means',
                  lcoe_dset='lcoe_fcr-means', h5_dsets=None, data_layers=None,
                  power_density=None, friction_fpath=None, friction_dset=None,
                  cap_cost_scale=None, recalc_lcoe=True):
-        """reV supply curve points aggregation framework.
+        r"""ReV supply curve points aggregation framework.
 
         ``reV`` supply curve aggregation combines a high-resolution
         (e.g. 90m) exclusion dataset with a (typically) lower resolution
         (e.g. 2km) generation dataset by mapping all data onto the high-
         resolution grid and aggregating it by a large factor (e.g. 64 or
         128). The result is coarsely-gridded data that summarizes
         capacity and generation potential as well as associated
@@ -323,14 +346,21 @@
                     },
                     "developable_land": {
                         "force_include_values": 42
                     },
                     "more_developable_land": {
                         "force_include_range": [5, 10]
                     },
+                    "viewsheds": {
+                        "exclude_values": 1,
+                        "extent": {
+                            "layer": "federal_parks",
+                            "include_range": [1, 5]
+                        }
+                    }
                     ...
                 }
 
             Note that all the keys given in this dictionary should be
             datasets of the `excl_fpath` file. If ``None`` or empty
             dictionary, no exclusions are applied. By default, ``None``.
         area_filter_kernel : {"queen", "rook"}, optional
@@ -646,100 +676,120 @@
                     inclusion mask (considers partial inclusions).
                 - category : dict
                     Dictionary mapping the unique values in the
                     `data_layer` to the sum of inclusion scalar values
                     associated with all pixels with that unique value.
         """
         log_versions(logger)
-        logger.info('Initializing SupplyCurveAggregation...')
-        logger.debug('Exclusion filepath: {}'.format(excl_fpath))
-        logger.debug('Exclusion dict: {}'.format(excl_dict))
-
-        super().__init__(excl_fpath, tm_dset, excl_dict=excl_dict,
-                         area_filter_kernel=area_filter_kernel,
-                         min_area=min_area, resolution=resolution,
-                         excl_area=excl_area, res_fpath=res_fpath, gids=gids,
-                         pre_extract_inclusions=pre_extract_inclusions)
+        logger.info("Initializing SupplyCurveAggregation...")
+        logger.debug("Exclusion filepath: {}".format(excl_fpath))
+        logger.debug("Exclusion dict: {}".format(excl_dict))
+
+        super().__init__(
+            excl_fpath,
+            tm_dset,
+            excl_dict=excl_dict,
+            area_filter_kernel=area_filter_kernel,
+            min_area=min_area,
+            resolution=resolution,
+            excl_area=excl_area,
+            res_fpath=res_fpath,
+            gids=gids,
+            pre_extract_inclusions=pre_extract_inclusions,
+        )
 
         self._econ_fpath = econ_fpath
         self._res_class_dset = res_class_dset
         self._res_class_bins = self._convert_bins(res_class_bins)
         self._cf_dset = cf_dset
         self._lcoe_dset = lcoe_dset
         self._h5_dsets = h5_dsets
         self._cap_cost_scale = cap_cost_scale
         self._power_density = power_density
         self._friction_fpath = friction_fpath
         self._friction_dset = friction_dset
         self._data_layers = data_layers
         self._recalc_lcoe = recalc_lcoe
 
-        logger.debug('Resource class bins: {}'.format(self._res_class_bins))
+        logger.debug("Resource class bins: {}".format(self._res_class_bins))
 
         if self._cap_cost_scale is not None:
             if self._h5_dsets is None:
                 self._h5_dsets = []
 
             self._h5_dsets += list(BaseGen.LCOE_ARGS)
             self._h5_dsets = list(set(self._h5_dsets))
 
         if self._power_density is None:
-            msg = ('Supply curve aggregation power density not specified. '
-                   'Will try to infer based on lookup table: {}'
-                   .format(GenerationSupplyCurvePoint.POWER_DENSITY))
+            msg = (
+                "Supply curve aggregation power density not specified. "
+                "Will try to infer based on lookup table: {}".format(
+                    GenerationSupplyCurvePoint.POWER_DENSITY
+                )
+            )
             logger.warning(msg)
             warn(msg, InputWarning)
 
         self._check_data_layers()
 
-    def _check_data_layers(self, methods=('mean', 'max', 'min',
-                           'mode', 'sum', 'category')):
+    def _check_data_layers(
+        self, methods=("mean", "max", "min", "mode", "sum", "category")
+    ):
         """Run pre-flight checks on requested aggregation data layers.
 
         Parameters
         ----------
         methods : list | tuple
             Data layer aggregation methods that are available to the user.
         """
 
         if self._data_layers is not None:
-            logger.debug('Checking data layers...')
+            logger.debug("Checking data layers...")
 
             with ExclusionLayers(self._excl_fpath) as f:
                 shape_base = f.shape
 
             for k, v in self._data_layers.items():
-                if 'dset' not in v:
-                    raise KeyError('Data aggregation "dset" data layer "{}" '
-                                   'must be specified.'.format(k))
-                if 'method' not in v:
-                    raise KeyError('Data aggregation "method" data layer "{}" '
-                                   'must be specified.'.format(k))
-                elif v['method'].lower() not in methods:
-                    raise ValueError('Cannot recognize data layer agg method: '
-                                     '"{}". Can only do: {}.'
-                                     .format(v['method'], methods))
-                if 'fpath' in v:
-                    with ExclusionLayers(v['fpath']) as f:
+                if "dset" not in v:
+                    raise KeyError(
+                        'Data aggregation "dset" data layer "{}" '
+                        "must be specified.".format(k)
+                    )
+                if "method" not in v:
+                    raise KeyError(
+                        'Data aggregation "method" data layer "{}" '
+                        "must be specified.".format(k)
+                    )
+                if v["method"].lower() not in methods:
+                    raise ValueError(
+                        "Cannot recognize data layer agg method: "
+                        '"{}". Can only do: {}.'.format(v["method"], methods)
+                    )
+                if "fpath" in v:
+                    with ExclusionLayers(v["fpath"]) as f:
                         try:
                             mismatched_shapes = any(f.shape != shape_base)
                         except TypeError:
                             mismatched_shapes = f.shape != shape_base
                         if mismatched_shapes:
-                            msg = ('Data shape of data layer "{}" is {}, '
-                                   'which does not match the baseline '
-                                   'exclusions shape {}.'
-                                   .format(k, f.shape, shape_base))
+                            msg = (
+                                'Data shape of data layer "{}" is {}, '
+                                "which does not match the baseline "
+                                "exclusions shape {}.".format(
+                                    k, f.shape, shape_base
+                                )
+                            )
                             raise FileInputError(msg)
 
-        logger.debug('Finished checking data layers.')
+        logger.debug("Finished checking data layers.")
 
     @staticmethod
-    def _get_res_gen_lcoe_data(gen, res_class_dset, res_class_bins,
-                               cf_dset, lcoe_dset):
+    def _get_res_gen_lcoe_data(
+        gen, res_class_dset, res_class_bins, cf_dset, lcoe_dset
+    ):
         """Extract the basic resource / generation / lcoe data to be used in
         the aggregation process.
 
         Parameters
         ----------
         gen : Resource | MultiFileResource
             Open rex resource handler initialized from gen_fpath and
@@ -765,35 +815,39 @@
             Capacity factor data extracted from cf_dset in gen
         lcoe_data : np.ndarray | None
             LCOE data extracted from lcoe_dset in gen
         """
 
         dset_list = (res_class_dset, cf_dset, lcoe_dset)
         gen_dsets = [] if gen is None else gen.datasets
-        labels = ('res_class_dset', 'cf_dset', 'lcoe_dset')
+        labels = ("res_class_dset", "cf_dset", "lcoe_dset")
         temp = [None, None, None]
 
         if isinstance(gen, Resource):
             source_fps = [gen.h5_file]
         elif isinstance(gen, MultiFileResource):
             source_fps = gen._h5_files
         else:
-            msg = ('Did not recognize gen object input of type "{}": {}'
-                   .format(type(gen), gen))
+            msg = 'Did not recognize gen object input of type "{}": {}'.format(
+                type(gen), gen
+            )
             logger.error(msg)
             raise TypeError(msg)
 
         for i, dset in enumerate(dset_list):
             if dset in gen_dsets:
                 _warn_about_large_datasets(gen, dset)
                 temp[i] = gen[dset]
             elif dset not in gen_dsets and dset is not None:
-                w = ('Could not find "{}" input as "{}" in source files: {}. '
-                     'Available datasets: {}'
-                     .format(labels[i], dset, source_fps, gen_dsets))
+                w = (
+                    'Could not find "{}" input as "{}" in source files: {}. '
+                    "Available datasets: {}".format(
+                        labels[i], dset, source_fps, gen_dsets
+                    )
+                )
                 logger.warning(w)
                 warn(w, OutputWarning)
 
         res_data, cf_data, lcoe_data = temp
 
         if res_class_dset is None or res_class_bins is None:
             res_class_bins = [None]
@@ -821,81 +875,113 @@
             keyed by the h5 dataset names. The corresponding values will be
             the extracted arrays from the h5 files.
         """
 
         # look for the datasets required by the LCOE re-calculation and make
         # lists of the missing datasets
         gen_dsets = [] if gen is None else gen.datasets
-        lcoe_recalc_req = ('fixed_charge_rate', 'capital_cost',
-                           'fixed_operating_cost', 'variable_operating_cost',
+        lcoe_recalc_req = ('fixed_charge_rate',
+                           'capital_cost',
+                           'fixed_operating_cost',
+                           'variable_operating_cost',
                            'system_capacity')
         missing_lcoe_source = [k for k in lcoe_recalc_req
                                if k not in gen_dsets]
         missing_lcoe_request = []
 
         if isinstance(gen, Resource):
             source_fps = [gen.h5_file]
         elif isinstance(gen, MultiFileResource):
             source_fps = gen._h5_files
         else:
-            msg = ('Did not recognize gen object input of type "{}": {}'
-                   .format(type(gen), gen))
+            msg = 'Did not recognize gen object input of type "{}": {}'.format(
+                type(gen), gen
+            )
             logger.error(msg)
             raise TypeError(msg)
 
         h5_dsets_data = None
         if h5_dsets is not None:
-            missing_lcoe_request = [k for k in lcoe_recalc_req
-                                    if k not in h5_dsets]
+            missing_lcoe_request = [
+                k for k in lcoe_recalc_req if k not in h5_dsets
+            ]
 
             if not isinstance(h5_dsets, (list, tuple)):
-                e = ('Additional h5_dsets argument must be a list or tuple '
-                     'but received: {} {}'.format(type(h5_dsets), h5_dsets))
+                e = (
+                    "Additional h5_dsets argument must be a list or tuple "
+                    "but received: {} {}".format(type(h5_dsets), h5_dsets)
+                )
                 logger.error(e)
                 raise TypeError(e)
 
             missing_h5_dsets = [k for k in h5_dsets if k not in gen_dsets]
             if any(missing_h5_dsets):
-                msg = ('Could not find requested h5_dsets "{}" in '
-                       'source files: {}. Available datasets: {}'
-                       .format(missing_h5_dsets, source_fps, gen_dsets))
+                msg = (
+                    'Could not find requested h5_dsets "{}" in '
+                    "source files: {}. Available datasets: {}".format(
+                        missing_h5_dsets, source_fps, gen_dsets
+                    )
+                )
                 logger.error(msg)
                 raise FileInputError(msg)
 
             h5_dsets_data = {dset: gen[dset] for dset in h5_dsets}
 
         if any(missing_lcoe_source):
-            msg = ('Could not find the datasets in the gen source file that '
-                   'are required to re-calculate the multi-year LCOE. If you '
-                   'are running a multi-year job, it is strongly suggested '
-                   'you pass through these datasets to re-calculate the LCOE '
-                   'from the multi-year mean CF: {}'
-                   .format(missing_lcoe_source))
+            msg = (
+                "Could not find the datasets in the gen source file that "
+                "are required to re-calculate the multi-year LCOE. If you "
+                "are running a multi-year job, it is strongly suggested "
+                "you pass through these datasets to re-calculate the LCOE "
+                "from the multi-year mean CF: {}".format(missing_lcoe_source)
+            )
             logger.warning(msg)
             warn(msg, InputWarning)
 
         if any(missing_lcoe_request):
-            msg = ('It is strongly advised that you include the following '
-                   'datasets in the h5_dsets request in order to re-calculate '
-                   'the LCOE from the multi-year mean CF and AEP: {}'
-                   .format(missing_lcoe_request))
+            msg = (
+                "It is strongly advised that you include the following "
+                "datasets in the h5_dsets request in order to re-calculate "
+                "the LCOE from the multi-year mean CF and AEP: {}".format(
+                    missing_lcoe_request
+                )
+            )
             logger.warning(msg)
             warn(msg, InputWarning)
 
         return h5_dsets_data
 
     @classmethod
-    def run_serial(cls, excl_fpath, gen_fpath, tm_dset, gen_index,
-                   econ_fpath=None, excl_dict=None, inclusion_mask=None,
-                   area_filter_kernel='queen', min_area=None,
-                   resolution=64, gids=None, args=None, res_class_dset=None,
-                   res_class_bins=None, cf_dset='cf_mean-means',
-                   lcoe_dset='lcoe_fcr-means', h5_dsets=None, data_layers=None,
-                   power_density=None, friction_fpath=None, friction_dset=None,
-                   excl_area=None, cap_cost_scale=None, recalc_lcoe=True):
+    def run_serial(
+        cls,
+        excl_fpath,
+        gen_fpath,
+        tm_dset,
+        gen_index,
+        econ_fpath=None,
+        excl_dict=None,
+        inclusion_mask=None,
+        area_filter_kernel="queen",
+        min_area=None,
+        resolution=64,
+        gids=None,
+        args=None,
+        res_class_dset=None,
+        res_class_bins=None,
+        cf_dset="cf_mean-means",
+        lcoe_dset="lcoe_fcr-means",
+        h5_dsets=None,
+        data_layers=None,
+        power_density=None,
+        friction_fpath=None,
+        friction_dset=None,
+        excl_area=None,
+        cap_cost_scale=None,
+        recalc_lcoe=True,
+    ):
         """Standalone method to create agg summary - can be parallelized.
 
         Parameters
         ----------
         excl_fpath : str | list | tuple
             Filepath to exclusions h5 with techmap dataset
             (can be one or more filepaths).
@@ -998,42 +1084,46 @@
             if gids is None:
                 gids = sc.valid_sc_points(tm_dset)
             elif np.issubdtype(type(gids), np.number):
                 gids = [gids]
 
             slice_lookup = sc.get_slice_lookup(gids)
 
-        logger.debug('Starting SupplyCurveAggregation serial with '
-                     'supply curve {} gids'.format(len(gids)))
+        logger.debug(
+            "Starting SupplyCurveAggregation serial with "
+            "supply curve {} gids".format(len(gids))
+        )
 
         cls._check_inclusion_mask(inclusion_mask, gids, exclusion_shape)
 
         # pre-extract handlers so they are not repeatedly initialized
-        file_kwargs = {'econ_fpath': econ_fpath,
-                       'data_layers': data_layers,
-                       'power_density': power_density,
-                       'excl_dict': excl_dict,
-                       'area_filter_kernel': area_filter_kernel,
-                       'min_area': min_area,
-                       'friction_fpath': friction_fpath,
-                       'friction_dset': friction_dset}
-        with SupplyCurveAggFileHandler(excl_fpath, gen_fpath,
-                                       **file_kwargs) as fh:
-
-            temp = cls._get_res_gen_lcoe_data(fh.gen, res_class_dset,
-                                              res_class_bins, cf_dset,
-                                              lcoe_dset)
+        file_kwargs = {
+            "econ_fpath": econ_fpath,
+            "data_layers": data_layers,
+            "power_density": power_density,
+            "excl_dict": excl_dict,
+            "area_filter_kernel": area_filter_kernel,
+            "min_area": min_area,
+            "friction_fpath": friction_fpath,
+            "friction_dset": friction_dset,
+        }
+        with SupplyCurveAggFileHandler(
+            excl_fpath, gen_fpath, **file_kwargs
+        ) as fh:
+            temp = cls._get_res_gen_lcoe_data(
+                fh.gen, res_class_dset, res_class_bins, cf_dset, lcoe_dset
+            )
             res_data, res_class_bins, cf_data, lcoe_data = temp
             h5_dsets_data = cls._get_extra_dsets(fh.gen, h5_dsets)
 
             n_finished = 0
             for gid in gids:
                 gid_inclusions = cls._get_gid_inclusion_mask(
-                    inclusion_mask, gid, slice_lookup,
-                    resolution=resolution)
+                    inclusion_mask, gid, slice_lookup, resolution=resolution
+                )
 
                 for ri, res_bin in enumerate(res_class_bins):
                     try:
                         pointsum = GenerationSupplyCurvePoint.summarize(
                             gid,
                             fh.exclusions,
                             fh.gen,
@@ -1051,35 +1141,42 @@
                             args=args,
                             excl_dict=excl_dict,
                             inclusion_mask=gid_inclusions,
                             excl_area=excl_area,
                             close=False,
                             friction_layer=fh.friction_layer,
                             cap_cost_scale=cap_cost_scale,
-                            recalc_lcoe=recalc_lcoe)
+                            recalc_lcoe=recalc_lcoe,
+                        )
 
                     except EmptySupplyCurvePointError:
-                        logger.debug('SC point {} is empty'.format(gid))
+                        logger.debug("SC point {} is empty".format(gid))
                     else:
-                        pointsum['sc_point_gid'] = gid
-                        pointsum['sc_row_ind'] = points.loc[gid, 'row_ind']
-                        pointsum['sc_col_ind'] = points.loc[gid, 'col_ind']
+                        pointsum[SupplyCurveField.SC_POINT_GID] = gid
+                        pointsum[SupplyCurveField.SC_ROW_IND] = \
+                            points.loc[gid, 'row_ind']
+                        pointsum[SupplyCurveField.SC_COL_IND] = \
+                            points.loc[gid, 'col_ind']
                         pointsum['res_class'] = ri
 
                         summary.append(pointsum)
-                        logger.debug('Serial aggregation completed gid {}: '
-                                     '{} out of {} points complete'
-                                     .format(gid, n_finished, len(gids)))
+                        logger.debug(
+                            "Serial aggregation completed gid {}: "
+                            "{} out of {} points complete".format(
+                                gid, n_finished, len(gids)
+                            )
+                        )
 
                 n_finished += 1
 
         return summary
 
-    def run_parallel(self, gen_fpath, args=None, max_workers=None,
-                     sites_per_worker=100):
+    def run_parallel(
+        self, gen_fpath, args=None, max_workers=None, sites_per_worker=100
+    ):
         """Get the supply curve points aggregation summary using futures.
 
         Parameters
         ----------
         gen_fpath : str
             Filepath to .h5 reV generation output results.
         args : tuple | list | None
@@ -1097,80 +1194,96 @@
             List of dictionaries, each being an SC point summary.
         """
 
         gen_index = self._parse_gen_index(gen_fpath)
         chunks = int(np.ceil(len(self.gids) / sites_per_worker))
         chunks = np.array_split(self.gids, chunks)
 
-        logger.info('Running supply curve point aggregation for '
-                    'points {} through {} at a resolution of {} '
-                    'on {} cores in {} chunks.'
-                    .format(self.gids[0], self.gids[-1], self._resolution,
-                            max_workers, len(chunks)))
+        logger.info(
+            "Running supply curve point aggregation for "
+            "points {} through {} at a resolution of {} "
+            "on {} cores in {} chunks.".format(
+                self.gids[0],
+                self.gids[-1],
+                self._resolution,
+                max_workers,
+                len(chunks),
+            )
+        )
 
         slice_lookup = None
         if self._inclusion_mask is not None:
-            with SupplyCurveExtent(self._excl_fpath,
-                                   resolution=self._resolution) as sc:
+            with SupplyCurveExtent(
+                self._excl_fpath, resolution=self._resolution
+            ) as sc:
                 assert sc.exclusions.shape == self._inclusion_mask.shape
                 slice_lookup = sc.get_slice_lookup(self.gids)
 
         futures = []
         summary = []
         n_finished = 0
-        loggers = [__name__, 'reV.supply_curve.point_summary', 'reV']
+        loggers = [__name__, "reV.supply_curve.point_summary", "reV"]
         with SpawnProcessPool(max_workers=max_workers, loggers=loggers) as exe:
-
             # iterate through split executions, submitting each to worker
             for gid_set in chunks:
                 # submit executions and append to futures list
                 chunk_incl_masks = None
                 if self._inclusion_mask is not None:
                     chunk_incl_masks = {}
                     for gid in gid_set:
                         rs, cs = slice_lookup[gid]
                         chunk_incl_masks[gid] = self._inclusion_mask[rs, cs]
 
-                futures.append(exe.submit(
-                    self.run_serial,
-                    self._excl_fpath, gen_fpath,
-                    self._tm_dset, gen_index,
-                    econ_fpath=self._econ_fpath,
-                    excl_dict=self._excl_dict,
-                    inclusion_mask=chunk_incl_masks,
-                    res_class_dset=self._res_class_dset,
-                    res_class_bins=self._res_class_bins,
-                    cf_dset=self._cf_dset,
-                    lcoe_dset=self._lcoe_dset,
-                    h5_dsets=self._h5_dsets,
-                    data_layers=self._data_layers,
-                    resolution=self._resolution,
-                    power_density=self._power_density,
-                    friction_fpath=self._friction_fpath,
-                    friction_dset=self._friction_dset,
-                    area_filter_kernel=self._area_filter_kernel,
-                    min_area=self._min_area,
-                    gids=gid_set,
-                    args=args,
-                    excl_area=self._excl_area,
-                    cap_cost_scale=self._cap_cost_scale,
-                    recalc_lcoe=self._recalc_lcoe))
+                futures.append(
+                    exe.submit(
+                        self.run_serial,
+                        self._excl_fpath,
+                        gen_fpath,
+                        self._tm_dset,
+                        gen_index,
+                        econ_fpath=self._econ_fpath,
+                        excl_dict=self._excl_dict,
+                        inclusion_mask=chunk_incl_masks,
+                        res_class_dset=self._res_class_dset,
+                        res_class_bins=self._res_class_bins,
+                        cf_dset=self._cf_dset,
+                        lcoe_dset=self._lcoe_dset,
+                        h5_dsets=self._h5_dsets,
+                        data_layers=self._data_layers,
+                        resolution=self._resolution,
+                        power_density=self._power_density,
+                        friction_fpath=self._friction_fpath,
+                        friction_dset=self._friction_dset,
+                        area_filter_kernel=self._area_filter_kernel,
+                        min_area=self._min_area,
+                        gids=gid_set,
+                        args=args,
+                        excl_area=self._excl_area,
+                        cap_cost_scale=self._cap_cost_scale,
+                        recalc_lcoe=self._recalc_lcoe,
+                    )
+                )
 
             # gather results
             for future in as_completed(futures):
                 n_finished += 1
                 summary += future.result()
                 if n_finished % 10 == 0:
                     mem = psutil.virtual_memory()
-                    logger.info('Parallel aggregation futures collected: '
-                                '{} out of {}. Memory usage is {:.3f} GB out '
-                                'of {:.3f} GB ({:.2f}% utilized).'
-                                .format(n_finished, len(chunks),
-                                        mem.used / 1e9, mem.total / 1e9,
-                                        100 * mem.used / mem.total))
+                    logger.info(
+                        "Parallel aggregation futures collected: "
+                        "{} out of {}. Memory usage is {:.3f} GB out "
+                        "of {:.3f} GB ({:.2f}% utilized).".format(
+                            n_finished,
+                            len(chunks),
+                            mem.used / 1e9,
+                            mem.total / 1e9,
+                            100 * mem.used / mem.total,
+                        )
+                    )
 
         return summary
 
     @staticmethod
     def _convert_bins(bins):
         """Convert a list of floats or ints to a list of two-entry bin bounds.
 
@@ -1190,25 +1303,26 @@
             return None
 
         type_check = [isinstance(x, (list, tuple)) for x in bins]
 
         if all(type_check):
             return bins
 
-        elif any(type_check):
-            raise TypeError('Resource class bins has inconsistent '
-                            'entry type: {}'.format(bins))
-
-        else:
-            bbins = []
-            for i, b in enumerate(sorted(bins)):
-                if i < len(bins) - 1:
-                    bbins.append([b, bins[i + 1]])
+        if any(type_check):
+            raise TypeError(
+                "Resource class bins has inconsistent "
+                "entry type: {}".format(bins)
+            )
+
+        bbins = []
+        for i, b in enumerate(sorted(bins)):
+            if i < len(bins) - 1:
+                bbins.append([b, bins[i + 1]])
 
-            return bbins
+        return bbins
 
     @staticmethod
     def _summary_to_df(summary):
         """Convert the agg summary list to a DataFrame.
 
         Parameters
         ----------
@@ -1217,23 +1331,25 @@
 
         Returns
         -------
         summary : DataFrame
             Summary of the SC points.
         """
         summary = pd.DataFrame(summary)
-        sort_by = [x for x in ('sc_point_gid', 'res_class') if x in summary]
+        sort_by = [x for x in (SupplyCurveField.SC_POINT_GID, 'res_class')
+                   if x in summary]
         summary = summary.sort_values(sort_by)
         summary = summary.reset_index(drop=True)
-        summary.index.name = 'sc_gid'
+        summary.index.name = SupplyCurveField.SC_GID
 
         return summary
 
-    def summarize(self, gen_fpath, args=None, max_workers=None,
-                  sites_per_worker=100):
+    def summarize(
+        self, gen_fpath, args=None, max_workers=None, sites_per_worker=100
+    ):
         """
         Get the supply curve points aggregation summary
 
         Parameters
         ----------
         gen_fpath : str
             Filepath to .h5 reV generation output results.
@@ -1253,52 +1369,68 @@
         """
         if max_workers is None:
             max_workers = os.cpu_count()
 
         if max_workers == 1:
             gen_index = self._parse_gen_index(gen_fpath)
             afk = self._area_filter_kernel
-            summary = self.run_serial(self._excl_fpath, gen_fpath,
-                                      self._tm_dset, gen_index,
-                                      econ_fpath=self._econ_fpath,
-                                      excl_dict=self._excl_dict,
-                                      inclusion_mask=self._inclusion_mask,
-                                      res_class_dset=self._res_class_dset,
-                                      res_class_bins=self._res_class_bins,
-                                      cf_dset=self._cf_dset,
-                                      lcoe_dset=self._lcoe_dset,
-                                      h5_dsets=self._h5_dsets,
-                                      data_layers=self._data_layers,
-                                      resolution=self._resolution,
-                                      power_density=self._power_density,
-                                      friction_fpath=self._friction_fpath,
-                                      friction_dset=self._friction_dset,
-                                      area_filter_kernel=afk,
-                                      min_area=self._min_area,
-                                      gids=self.gids, args=args,
-                                      excl_area=self._excl_area,
-                                      cap_cost_scale=self._cap_cost_scale,
-                                      recalc_lcoe=self._recalc_lcoe)
+            summary = self.run_serial(
+                self._excl_fpath,
+                gen_fpath,
+                self._tm_dset,
+                gen_index,
+                econ_fpath=self._econ_fpath,
+                excl_dict=self._excl_dict,
+                inclusion_mask=self._inclusion_mask,
+                res_class_dset=self._res_class_dset,
+                res_class_bins=self._res_class_bins,
+                cf_dset=self._cf_dset,
+                lcoe_dset=self._lcoe_dset,
+                h5_dsets=self._h5_dsets,
+                data_layers=self._data_layers,
+                resolution=self._resolution,
+                power_density=self._power_density,
+                friction_fpath=self._friction_fpath,
+                friction_dset=self._friction_dset,
+                area_filter_kernel=afk,
+                min_area=self._min_area,
+                gids=self.gids,
+                args=args,
+                excl_area=self._excl_area,
+                cap_cost_scale=self._cap_cost_scale,
+                recalc_lcoe=self._recalc_lcoe,
+            )
         else:
-            summary = self.run_parallel(gen_fpath=gen_fpath, args=args,
-                                        max_workers=max_workers,
-                                        sites_per_worker=sites_per_worker)
+            summary = self.run_parallel(
+                gen_fpath=gen_fpath,
+                args=args,
+                max_workers=max_workers,
+                sites_per_worker=sites_per_worker,
+            )
 
         if not any(summary):
-            e = ('Supply curve aggregation found no non-excluded SC points. '
-                 'Please check your exclusions or subset SC GID selection.')
+            e = (
+                "Supply curve aggregation found no non-excluded SC points. "
+                "Please check your exclusions or subset SC GID selection."
+            )
             logger.error(e)
             raise EmptySupplyCurvePointError(e)
 
         summary = self._summary_to_df(summary)
 
         return summary
 
-    def run(self, out_fpath, gen_fpath=None, args=None, max_workers=None,
-            sites_per_worker=100):
+    def run(
+        self,
+        out_fpath,
+        gen_fpath=None,
+        args=None,
+        max_workers=None,
+        sites_per_worker=100,
+    ):
         """Run a supply curve aggregation.
 
         Parameters
         ----------
         gen_fpath : str, optional
             Filepath to HDF5 file with ``reV`` generation output
             results. If ``None``, a simple aggregation without any
@@ -1329,49 +1461,58 @@
         -------
         str
             Path to output CSV file containing supply curve aggregation.
         """
 
         if gen_fpath is None:
             out = Aggregation.run(
-                self._excl_fpath, self._res_fpath, self._tm_dset,
+                self._excl_fpath,
+                self._res_fpath,
+                self._tm_dset,
                 excl_dict=self._excl_dict,
                 resolution=self._resolution,
                 excl_area=self._excl_area,
                 area_filter_kernel=self._area_filter_kernel,
                 min_area=self._min_area,
                 pre_extract_inclusions=self._pre_extract_inclusions,
                 max_workers=max_workers,
-                sites_per_worker=sites_per_worker)
-            summary = out['meta']
+                sites_per_worker=sites_per_worker,
+            )
+            summary = out["meta"]
         else:
-            summary = self.summarize(gen_fpath=gen_fpath, args=args,
-                                     max_workers=max_workers,
-                                     sites_per_worker=sites_per_worker)
+            summary = self.summarize(
+                gen_fpath=gen_fpath,
+                args=args,
+                max_workers=max_workers,
+                sites_per_worker=sites_per_worker,
+            )
 
         out_fpath = _format_sc_agg_out_fpath(out_fpath)
         summary.to_csv(out_fpath)
 
         return out_fpath
 
 
 def _format_sc_agg_out_fpath(out_fpath):
     """Add CSV file ending and replace underscore, if necessary."""
     if not out_fpath.endswith(".csv"):
-        out_fpath = '{}.csv'.format(out_fpath)
+        out_fpath = "{}.csv".format(out_fpath)
 
     project_dir, out_fn = os.path.split(out_fpath)
-    out_fn = out_fn.replace("supply_curve_aggregation",
-                            "supply-curve-aggregation")
+    out_fn = out_fn.replace(
+        "supply_curve_aggregation", "supply-curve-aggregation"
+    )
     return os.path.join(project_dir, out_fn)
 
 
 def _warn_about_large_datasets(gen, dset):
     """Warn user about multi-dimensional datasets in passthrough datasets"""
     dset_shape = gen.shapes.get(dset, (1,))
     if len(dset_shape) > 1:
-        msg = ("Generation dataset {!r} is not 1-dimensional (shape: {})."
-               "You may run into memory errors during aggregation - use "
-               "rep-profiles for aggregating higher-order datasets instead!"
-               .format(dset, dset_shape))
+        msg = (
+            "Generation dataset {!r} is not 1-dimensional (shape: {})."
+            "You may run into memory errors during aggregation - use "
+            "rep-profiles for aggregating higher-order datasets instead!"
+            .format(dset, dset_shape)
+        )
         logger.warning(msg)
         warn(msg, UserWarning)
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/supply_curve.py` & `NREL-reV-0.8.9/reV/supply_curve/supply_curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 reV supply curve module
 - Calculation of LCOT
 - Supply Curve creation
 """
-from copy import deepcopy
 import json
 import logging
-import numpy as np
 import os
-import pandas as pd
+from copy import deepcopy
 from warnings import warn
 
+import numpy as np
+import pandas as pd
+from rex import Resource
+from rex.utilities import SpawnProcessPool, parse_table
+
 from reV.handlers.transmission import TransmissionCosts as TC
 from reV.handlers.transmission import TransmissionFeatures as TF
 from reV.supply_curve.competitive_wind_farms import CompetitiveWindFarms
-from reV.utilities.exceptions import SupplyCurveInputError, SupplyCurveError
-from reV.utilities import log_versions
-
-from rex import Resource
-from rex.utilities import parse_table, SpawnProcessPool
-
+from reV.utilities import SupplyCurveField, log_versions
+from reV.utilities.exceptions import SupplyCurveError, SupplyCurveInputError
 
 logger = logging.getLogger(__name__)
 
 
 class SupplyCurve:
     """SupplyCurve"""
 
     def __init__(self, sc_points, trans_table, sc_features=None,
-                 sc_capacity_col='capacity'):
-        """reV LCOT calculation and SupplyCurve sorting class.
+                 sc_capacity_col=SupplyCurveField.CAPACITY):
+        """ReV LCOT calculation and SupplyCurve sorting class.
 
         ``reV`` supply curve computes the transmission costs associated
         with each supply curve point output by ``reV`` supply curve
         aggregation. Transmission costs can either be computed
         competitively (where total capacity remaining on the
         transmission grid is tracked and updated after each new
         connection) or non-competitively (where the cheapest connections
@@ -123,23 +122,25 @@
                 ($/MWh).
             - total_lcoe_friction : float
                 Total LCOE of each supply curve point considering the
                 LCOE friction scalar from the aggregation step
                 (mean_lcoe_friction + lcot) ($/MWh).
         """
         log_versions(logger)
-        logger.info('Supply curve points input: {}'.format(sc_points))
-        logger.info('Transmission table input: {}'.format(trans_table))
-        logger.info('Supply curve capacity column: {}'.format(sc_capacity_col))
+        logger.info("Supply curve points input: {}".format(sc_points))
+        logger.info("Transmission table input: {}".format(trans_table))
+        logger.info("Supply curve capacity column: {}".format(sc_capacity_col))
 
         self._sc_capacity_col = sc_capacity_col
-        self._sc_points = self._parse_sc_points(sc_points,
-                                                sc_features=sc_features)
-        self._trans_table = self._map_tables(self._sc_points, trans_table,
-                                             sc_capacity_col=sc_capacity_col)
+        self._sc_points = self._parse_sc_points(
+            sc_points, sc_features=sc_features
+        )
+        self._trans_table = self._map_tables(
+            self._sc_points, trans_table, sc_capacity_col=sc_capacity_col
+        )
         self._sc_gids, self._mask = self._parse_sc_gids(self._trans_table)
 
     def __repr__(self):
         msg = "{} with {} points".format(self.__class__.__name__, len(self))
 
         return msg
 
@@ -173,39 +174,51 @@
 
         Returns
         -------
         sc_points : pandas.DataFrame
             DataFrame of supply curve point summary with additional features
             added if supplied
         """
-        if isinstance(sc_points, str) and sc_points.endswith('.h5'):
+        if isinstance(sc_points, str) and sc_points.endswith(".h5"):
             with Resource(sc_points) as res:
                 sc_points = res.meta
-                sc_points.index.name = 'sc_gid'
+                sc_points.index.name = SupplyCurveField.SC_GID
                 sc_points = sc_points.reset_index()
         else:
             sc_points = parse_table(sc_points)
+            sc_points = sc_points.rename(
+                columns=SupplyCurveField.map_from_legacy())
 
-        logger.debug('Supply curve points table imported with columns: {}'
-                     .format(sc_points.columns.values.tolist()))
+        logger.debug(
+            "Supply curve points table imported with columns: {}".format(
+                sc_points.columns.values.tolist()
+            )
+        )
 
         if sc_features is not None:
             sc_features = parse_table(sc_features)
-            merge_cols = [c for c in sc_features
-                          if c in sc_points]
-            sc_points = sc_points.merge(sc_features, on=merge_cols, how='left')
-            logger.debug('Adding Supply Curve Features table with columns: {}'
-                         .format(sc_features.columns.values.tolist()))
+            sc_features = sc_features.rename(
+                columns=SupplyCurveField.map_from_legacy())
+            merge_cols = [c for c in sc_features if c in sc_points]
+            sc_points = sc_points.merge(sc_features, on=merge_cols, how="left")
+            logger.debug(
+                "Adding Supply Curve Features table with columns: {}".format(
+                    sc_features.columns.values.tolist()
+                )
+            )
 
-        if 'transmission_multiplier' in sc_points:
-            col = 'transmission_multiplier'
+        if "transmission_multiplier" in sc_points:
+            col = "transmission_multiplier"
             sc_points.loc[:, col] = sc_points.loc[:, col].fillna(1)
 
-        logger.debug('Final supply curve points table has columns: {}'
-                     .format(sc_points.columns.values.tolist()))
+        logger.debug(
+            "Final supply curve points table has columns: {}".format(
+                sc_points.columns.values.tolist()
+            )
+        )
 
         return sc_points
 
     @staticmethod
     def _get_merge_cols(sc_columns, trans_columns):
         """
         Get columns with 'row' or 'col' in them to use for merging
@@ -218,26 +231,28 @@
 
         Returns
         -------
         merge_cols : dict
             Columns to merge on which maps the sc columns (keys) to the
             corresponding trans table columns (values)
         """
-        sc_columns = [c for c in sc_columns if c.startswith('sc_')]
-        trans_columns = [c for c in trans_columns if c.startswith('sc_')]
+        sc_columns = [c for c in sc_columns if c.startswith("sc_")]
+        trans_columns = [c for c in trans_columns if c.startswith("sc_")]
         merge_cols = {}
-        for c_val in ['row', 'col']:
+        for c_val in ["row", "col"]:
             trans_col = [c for c in trans_columns if c_val in c]
             sc_col = [c for c in sc_columns if c_val in c]
             if trans_col and sc_col:
                 merge_cols[sc_col[0]] = trans_col[0]
 
         if len(merge_cols) != 2:
-            msg = ('Did not find a unique set of sc row and column ids to '
-                   'merge on: {}'.format(merge_cols))
+            msg = (
+                "Did not find a unique set of sc row and column ids to "
+                "merge on: {}".format(merge_cols)
+            )
             logger.error(msg)
             raise RuntimeError(msg)
 
         return merge_cols
 
     @staticmethod
     def _parse_trans_table(trans_table):
@@ -262,32 +277,36 @@
         # column names:
         # trans_gid -> the transmission feature id, legacy name: trans_line_gid
         # trans_line_gids -> gids of transmission lines connected to the given
         # transmission feature (only used for Substations),
         # legacy name: trans_gids
         # also xformer_cost_p_mw -> xformer_cost_per_mw (not sure why there
         # would be a *_p_mw but here we are...)
-        rename_map = {'trans_line_gid': 'trans_gid',
-                      'trans_gids': 'trans_line_gids',
-                      'xformer_cost_p_mw': 'xformer_cost_per_mw'}
+        rename_map = {
+            "trans_line_gid": "trans_gid",
+            "trans_gids": "trans_line_gids",
+            "xformer_cost_p_mw": "xformer_cost_per_mw",
+        }
         trans_table = trans_table.rename(columns=rename_map)
 
-        if 'dist_mi' in trans_table and 'dist_km' not in trans_table:
-            trans_table = trans_table.rename(columns={'dist_mi': 'dist_km'})
-            trans_table['dist_km'] *= 1.60934
+        if "dist_mi" in trans_table and "dist_km" not in trans_table:
+            trans_table = trans_table.rename(columns={"dist_mi": "dist_km"})
+            trans_table["dist_km"] *= 1.60934
 
-        drop_cols = ['sc_gid', 'cap_left', 'sc_point_gid']
+        drop_cols = [SupplyCurveField.SC_GID, 'cap_left',
+                     SupplyCurveField.SC_POINT_GID]
         drop_cols = [c for c in drop_cols if c in trans_table]
         if drop_cols:
             trans_table = trans_table.drop(columns=drop_cols)
 
-        return trans_table
+        return trans_table.rename(columns=SupplyCurveField.map_from_legacy())
 
     @staticmethod
-    def _map_trans_capacity(trans_sc_table, sc_capacity_col='capacity'):
+    def _map_trans_capacity(trans_sc_table,
+                            sc_capacity_col=SupplyCurveField.CAPACITY):
         """
         Map SC gids to transmission features based on capacity. For any SC
         gids with capacity > the maximum transmission feature capacity, map
         SC gids to the feature with the largest capacity
 
         Parameters
         ----------
@@ -306,41 +325,50 @@
         Returns
         -------
         trans_sc_table : pandas.DataFrame
             Updated table mapping supply curve points to transmission features
             based on maximum capacity
         """
 
-        nx = trans_sc_table[sc_capacity_col] / trans_sc_table['max_cap']
+        nx = trans_sc_table[sc_capacity_col] / trans_sc_table["max_cap"]
         nx = np.ceil(nx).astype(int)
-        trans_sc_table['n_parallel_trans'] = nx
+        trans_sc_table["n_parallel_trans"] = nx
 
         if (nx > 1).any():
             mask = nx > 1
-            tie_line_cost = (trans_sc_table.loc[mask, 'tie_line_cost']
-                             * nx[mask])
-
-            xformer_cost = (trans_sc_table.loc[mask, 'xformer_cost_per_mw']
-                            * trans_sc_table.loc[mask, 'max_cap'] * nx[mask])
-
-            conn_cost = (xformer_cost
-                         + trans_sc_table.loc[mask, 'sub_upgrade_cost']
-                         + trans_sc_table.loc[mask, 'new_sub_cost'])
+            tie_line_cost = (
+                trans_sc_table.loc[mask, "tie_line_cost"] * nx[mask]
+            )
+
+            xformer_cost = (
+                trans_sc_table.loc[mask, "xformer_cost_per_mw"]
+                * trans_sc_table.loc[mask, "max_cap"]
+                * nx[mask]
+            )
+
+            conn_cost = (
+                xformer_cost
+                + trans_sc_table.loc[mask, "sub_upgrade_cost"]
+                + trans_sc_table.loc[mask, "new_sub_cost"]
+            )
 
             trans_cap_cost = tie_line_cost + conn_cost
 
-            trans_sc_table.loc[mask, 'tie_line_cost'] = tie_line_cost
-            trans_sc_table.loc[mask, 'xformer_cost'] = xformer_cost
-            trans_sc_table.loc[mask, 'connection_cost'] = conn_cost
-            trans_sc_table.loc[mask, 'trans_cap_cost'] = trans_cap_cost
-
-            msg = ("{} SC points have a capacity that exceeds the maximum "
-                   "transmission feature capacity and will be connected with "
-                   "multiple parallel transmission features."
-                   .format((nx > 1).sum()))
+            trans_sc_table.loc[mask, "tie_line_cost"] = tie_line_cost
+            trans_sc_table.loc[mask, "xformer_cost"] = xformer_cost
+            trans_sc_table.loc[mask, "connection_cost"] = conn_cost
+            trans_sc_table.loc[mask, "trans_cap_cost"] = trans_cap_cost
+
+            msg = (
+                "{} SC points have a capacity that exceeds the maximum "
+                "transmission feature capacity and will be connected with "
+                "multiple parallel transmission features.".format(
+                    (nx > 1).sum()
+                )
+            )
             logger.info(msg)
 
         return trans_sc_table
 
     @staticmethod
     def _parse_trans_line_gids(trans_line_gids):
         """
@@ -375,57 +403,66 @@
 
         Returns
         -------
         line_gids : list
             List of missing transmission line 'trans_gid's for all substations
             in features table
         """
-        features = features.rename(columns={'trans_line_gid': 'trans_gid',
-                                            'trans_gids': 'trans_line_gids'})
-        mask = features['category'].str.lower() == 'substation'
+        features = features.rename(
+            columns={
+                "trans_line_gid": "trans_gid",
+                "trans_gids": "trans_line_gids",
+            }
+        )
+        mask = features["category"].str.lower() == "substation"
 
         if not any(mask):
             return []
 
-        line_gids = (features.loc[mask, 'trans_line_gids']
-                     .apply(cls._parse_trans_line_gids))
+        line_gids = features.loc[mask, "trans_line_gids"].apply(
+            cls._parse_trans_line_gids
+        )
 
         line_gids = np.unique(np.concatenate(line_gids.values))
 
-        test = np.isin(line_gids, features['trans_gid'].values)
+        test = np.isin(line_gids, features["trans_gid"].values)
 
         return line_gids[~test].tolist()
 
     @classmethod
-    def _check_substation_conns(cls, trans_table, sc_cols='sc_gid'):
+    def _check_substation_conns(cls, trans_table,
+                                sc_cols=SupplyCurveField.SC_GID):
         """
         Run checks on substation transmission features to make sure that
         every sc point connecting to a substation can also connect to its
         respective transmission lines
 
         Parameters
         ----------
         trans_table : pd.DataFrame
             Table mapping supply curve points to transmission features
             (should already be merged with SC points).
         sc_cols : str | list, optional
             Column(s) in trans_table with unique supply curve id,
-            by default 'sc_gid'
+            by default SupplyCurveField.SC_GID
         """
         missing = {}
         for sc_point, sc_table in trans_table.groupby(sc_cols):
             tl_gids = cls._check_sub_trans_lines(sc_table)
             if tl_gids:
                 missing[sc_point] = tl_gids
 
         if any(missing):
-            msg = ('The following sc_gid (keys) were connected to substations '
-                   'but were not connected to the respective transmission line'
-                   ' gids (values) which is required for full SC sort: {}'
-                   .format(missing))
+            msg = (
+                "The following sc_gid (keys) were connected to substations "
+                "but were not connected to the respective transmission line"
+                " gids (values) which is required for full SC sort: {}".format(
+                    missing
+                )
+            )
             logger.error(msg)
             raise SupplyCurveInputError(msg)
 
     @classmethod
     def _check_sc_trans_table(cls, sc_points, trans_table):
         """Run self checks on sc_points table and the merged trans_table
 
@@ -433,60 +470,73 @@
         ----------
         sc_points : pd.DataFrame
             Table of supply curve point summary
         trans_table : pd.DataFrame
             Table mapping supply curve points to transmission features
             (should already be merged with SC points).
         """
-        sc_gids = set(sc_points['sc_gid'].unique())
-        trans_sc_gids = set(trans_table['sc_gid'].unique())
+        sc_gids = set(sc_points[SupplyCurveField.SC_GID].unique())
+        trans_sc_gids = set(trans_table[SupplyCurveField.SC_GID].unique())
         missing = sorted(list(sc_gids - trans_sc_gids))
         if any(missing):
-            msg = ("There are {} Supply Curve points with missing "
-                   "transmission mappings. Supply curve points with no "
-                   "transmission features will not be connected! "
-                   "Missing sc_gid's: {}"
-                   .format(len(missing), missing))
+            msg = (
+                "There are {} Supply Curve points with missing "
+                "transmission mappings. Supply curve points with no "
+                "transmission features will not be connected! "
+                "Missing sc_gid's: {}".format(len(missing), missing)
+            )
             logger.warning(msg)
             warn(msg)
 
         if not any(trans_sc_gids) or not any(sc_gids):
-            msg = ('Merging of sc points table and transmission features '
-                   'table failed with {} original sc gids and {} transmission '
-                   'sc gids after table merge.'
-                   .format(len(sc_gids), len(trans_sc_gids)))
+            msg = (
+                "Merging of sc points table and transmission features "
+                "table failed with {} original sc gids and {} transmission "
+                "sc gids after table merge.".format(
+                    len(sc_gids), len(trans_sc_gids)
+                )
+            )
             logger.error(msg)
             raise SupplyCurveError(msg)
 
-        logger.debug('There are {} original SC gids and {} sc gids in the '
-                     'merged transmission table.'
-                     .format(len(sc_gids), len(trans_sc_gids)))
-        logger.debug('Transmission Table created with columns: {}'
-                     .format(trans_table.columns.values.tolist()))
+        logger.debug(
+            "There are {} original SC gids and {} sc gids in the "
+            "merged transmission table.".format(
+                len(sc_gids), len(trans_sc_gids)
+            )
+        )
+        logger.debug(
+            "Transmission Table created with columns: {}".format(
+                trans_table.columns.values.tolist()
+            )
+        )
 
     @classmethod
     def _merge_sc_trans_tables(cls, sc_points, trans_table,
-                               sc_cols=('sc_gid', 'capacity', 'mean_cf',
-                                        'mean_lcoe'),
-                               sc_capacity_col='capacity'):
+                               sc_cols=(SupplyCurveField.SC_GID,
+                                        SupplyCurveField.CAPACITY,
+                                        SupplyCurveField.MEAN_CF,
+                                        SupplyCurveField.MEAN_LCOE),
+                               sc_capacity_col=SupplyCurveField.CAPACITY):
         """
         Merge the supply curve table with the transmission features table.
 
         Parameters
         ----------
         sc_points : pd.DataFrame
             Table of supply curve point summary
         trans_table : pd.DataFrame | str
             Table mapping supply curve points to transmission features
             (either str filepath to table file, list of filepaths to tables by
              line voltage (capacity) or pre-loaded dataframe).
         sc_cols : tuple | list, optional
             List of column from sc_points to transfer into the trans table,
             If the `sc_capacity_col` is not included, it will get added.
-            by default ('sc_gid', 'capacity', 'mean_cf', 'mean_lcoe')
+            by default (SupplyCurveField.SC_GID, 'capacity', 'mean_cf',
+            'mean_lcoe')
         sc_capacity_col : str, optional
             Name of capacity column in `trans_sc_table`. The values in
             this column determine the size of transmission lines built.
             The transmission capital costs per MW and the reinforcement
             costs per MW will be returned in terms of these capacity
             values. Note that if this column != "capacity", then
             "capacity" must also be included in `trans_sc_table` since
@@ -501,65 +551,79 @@
         """
         if sc_capacity_col not in sc_cols:
             sc_cols = tuple([sc_capacity_col] + list(sc_cols))
 
         if isinstance(trans_table, (list, tuple)):
             trans_sc_table = []
             for table in trans_table:
-                trans_sc_table.append(cls._merge_sc_trans_tables(
-                    sc_points, table, sc_cols=sc_cols,
-                    sc_capacity_col=sc_capacity_col))
+                trans_sc_table.append(
+                    cls._merge_sc_trans_tables(
+                        sc_points,
+                        table,
+                        sc_cols=sc_cols,
+                        sc_capacity_col=sc_capacity_col,
+                    )
+                )
 
             trans_sc_table = pd.concat(trans_sc_table)
         else:
             trans_table = cls._parse_trans_table(trans_table)
 
-            merge_cols = cls._get_merge_cols(sc_points.columns,
-                                             trans_table.columns)
-            logger.info('Merging SC table and Trans Table with '
-                        '{} mapping: {}'
-                        .format('sc_table_col: trans_table_col', merge_cols))
+            merge_cols = cls._get_merge_cols(
+                sc_points.columns, trans_table.columns
+            )
+            logger.info(
+                "Merging SC table and Trans Table with "
+                "{} mapping: {}".format(
+                    "sc_table_col: trans_table_col", merge_cols
+                )
+            )
             sc_points = sc_points.rename(columns=merge_cols)
             merge_cols = list(merge_cols.values())
 
             if isinstance(sc_cols, tuple):
                 sc_cols = list(sc_cols)
 
-            if 'mean_lcoe_friction' in sc_points:
-                sc_cols.append('mean_lcoe_friction')
+            if SupplyCurveField.MEAN_LCOE_FRICTION in sc_points:
+                sc_cols.append(SupplyCurveField.MEAN_LCOE_FRICTION)
 
-            if 'transmission_multiplier' in sc_points:
-                sc_cols.append('transmission_multiplier')
+            if "transmission_multiplier" in sc_points:
+                sc_cols.append("transmission_multiplier")
 
             sc_cols += merge_cols
             sc_points = sc_points[sc_cols].copy()
-            trans_sc_table = trans_table.merge(sc_points, on=merge_cols,
-                                               how='inner')
+            trans_sc_table = trans_table.merge(
+                sc_points, on=merge_cols, how="inner"
+            )
 
         return trans_sc_table
 
     @classmethod
     def _map_tables(cls, sc_points, trans_table,
-                    sc_cols=('sc_gid', 'capacity', 'mean_cf', 'mean_lcoe'),
-                    sc_capacity_col='capacity'):
+                    sc_cols=(SupplyCurveField.SC_GID,
+                             SupplyCurveField.CAPACITY,
+                             SupplyCurveField.MEAN_CF,
+                             SupplyCurveField.MEAN_LCOE),
+                    sc_capacity_col=SupplyCurveField.CAPACITY):
         """
         Map supply curve points to transmission features
 
         Parameters
         ----------
         sc_points : pd.DataFrame
             Table of supply curve point summary
         trans_table : pd.DataFrame | str
             Table mapping supply curve points to transmission features
             (either str filepath to table file, list of filepaths to tables by
              line voltage (capacity) or pre-loaded DataFrame).
         sc_cols : tuple | list, optional
             List of column from sc_points to transfer into the trans table,
             If the `sc_capacity_col` is not included, it will get added.
-            by default ('sc_gid', 'capacity', 'mean_cf', 'mean_lcoe')
+            by default (SupplyCurveField.SC_GID, SupplyCurveField.CAPACITY,
+            SupplyCurveField.MEAN_CF, SupplyCurveField.MEAN_LCOE)
         sc_capacity_col : str, optional
             Name of capacity column in `trans_sc_table`. The values in
             this column determine the size of transmission lines built.
             The transmission capital costs per MW and the reinforcement
             costs per MW will be returned in terms of these capacity
             values. Note that if this column != "capacity", then
             "capacity" must also be included in `trans_sc_table` since
@@ -569,25 +633,26 @@
         Returns
         -------
         trans_sc_table : pd.DataFrame
             Updated table mapping supply curve points to transmission features.
             This is performed by an inner merging with trans_table
         """
         scc = sc_capacity_col
-        trans_sc_table = cls._merge_sc_trans_tables(sc_points, trans_table,
-                                                    sc_cols=sc_cols,
-                                                    sc_capacity_col=scc)
-
-        if 'max_cap' in trans_sc_table:
-            trans_sc_table = cls._map_trans_capacity(trans_sc_table,
-                                                     sc_capacity_col=scc)
+        trans_sc_table = cls._merge_sc_trans_tables(
+            sc_points, trans_table, sc_cols=sc_cols, sc_capacity_col=scc
+        )
+
+        if "max_cap" in trans_sc_table:
+            trans_sc_table = cls._map_trans_capacity(
+                trans_sc_table, sc_capacity_col=scc
+            )
 
         trans_sc_table = \
             trans_sc_table.sort_values(
-                ['sc_gid', 'trans_gid']).reset_index(drop=True)
+                [SupplyCurveField.SC_GID, 'trans_gid']).reset_index(drop=True)
 
         cls._check_sc_trans_table(sc_points, trans_sc_table)
 
         return trans_sc_table
 
     @staticmethod
     def _create_handler(trans_table, trans_costs=None, avail_cap_frac=1):
@@ -615,21 +680,22 @@
             with specified transmission costs
         """
         if trans_costs is not None:
             kwargs = TF._parse_dictionary(trans_costs)
         else:
             kwargs = {}
 
-        trans_features = TF(trans_table, avail_cap_frac=avail_cap_frac,
-                            **kwargs)
+        trans_features = TF(
+            trans_table, avail_cap_frac=avail_cap_frac, **kwargs
+        )
 
         return trans_features
 
     @staticmethod
-    def _parse_sc_gids(trans_table, gid_key='sc_gid'):
+    def _parse_sc_gids(trans_table, gid_key=SupplyCurveField.SC_GID):
         """Extract unique sc gids, make bool mask from tranmission table
 
         Parameters
         ----------
         trans_table : pd.DataFrame
             reV Supply Curve table joined with transmission features table.
         gid_key : str
@@ -648,15 +714,15 @@
         sc_gids = [int(gid) for gid in sc_gids]
         mask = np.ones(int(1 + max(sc_gids)), dtype=bool)
 
         return sc_gids, mask
 
     @staticmethod
     def _get_capacity(sc_gid, sc_table, connectable=True,
-                      sc_capacity_col='capacity'):
+                      sc_capacity_col=SupplyCurveField.CAPACITY):
         """
         Get capacity of supply curve point
 
         Parameters
         ----------
         sc_gid : int
             Supply curve gid
@@ -682,29 +748,30 @@
             Capacity of supply curve point
         """
         if connectable:
             capacity = sc_table[sc_capacity_col].unique()
             if len(capacity) == 1:
                 capacity = capacity[0]
             else:
-                msg = ('Each supply curve point should only have '
-                       'a single capacity, but {} has {}'
-                       .format(sc_gid, capacity))
+                msg = (
+                    "Each supply curve point should only have "
+                    "a single capacity, but {} has {}".format(sc_gid, capacity)
+                )
                 logger.error(msg)
                 raise RuntimeError(msg)
         else:
             capacity = None
 
         return capacity
 
     @classmethod
     def _compute_trans_cap_cost(cls, trans_table, trans_costs=None,
                                 avail_cap_frac=1, max_workers=None,
                                 connectable=True, line_limited=False,
-                                sc_capacity_col='capacity'):
+                                sc_capacity_col=SupplyCurveField.CAPACITY):
         """
         Compute levelized cost of transmission for all combinations of
         supply curve points and tranmission features in trans_table
 
         Parameters
         ----------
         trans_table : pd.DataFrame
@@ -745,65 +812,89 @@
             tranmission feature connections
         cost : list
             Capital cost of tramsmission for all supply curve - transmission
             feature connections
         """
         scc = sc_capacity_col
         if scc not in trans_table:
-            raise SupplyCurveInputError('Supply curve table must have '
-                                        'supply curve point capacity column'
-                                        '({}) to compute lcot'.format(scc))
+            raise SupplyCurveInputError(
+                "Supply curve table must have "
+                "supply curve point capacity column"
+                "({}) to compute lcot".format(scc)
+            )
 
         if trans_costs is not None:
             trans_costs = TF._parse_dictionary(trans_costs)
         else:
             trans_costs = {}
 
         if max_workers is None:
             max_workers = os.cpu_count()
 
         logger.info('Computing LCOT costs for all possible connections...')
-        groups = trans_table.groupby('sc_gid')
+        groups = trans_table.groupby(SupplyCurveField.SC_GID)
         if max_workers > 1:
-            loggers = [__name__, 'reV.handlers.transmission', 'reV']
-            with SpawnProcessPool(max_workers=max_workers,
-                                  loggers=loggers) as exe:
+            loggers = [__name__, "reV.handlers.transmission", "reV"]
+            with SpawnProcessPool(
+                max_workers=max_workers, loggers=loggers
+            ) as exe:
                 futures = []
                 for sc_gid, sc_table in groups:
-                    capacity = cls._get_capacity(sc_gid, sc_table,
-                                                 connectable=connectable,
-                                                 sc_capacity_col=scc)
-                    futures.append(exe.submit(TC.feature_costs, sc_table,
-                                              capacity=capacity,
-                                              avail_cap_frac=avail_cap_frac,
-                                              line_limited=line_limited,
-                                              **trans_costs))
+                    capacity = cls._get_capacity(
+                        sc_gid,
+                        sc_table,
+                        connectable=connectable,
+                        sc_capacity_col=scc,
+                    )
+                    futures.append(
+                        exe.submit(
+                            TC.feature_costs,
+                            sc_table,
+                            capacity=capacity,
+                            avail_cap_frac=avail_cap_frac,
+                            line_limited=line_limited,
+                            **trans_costs,
+                        )
+                    )
 
                 cost = [future.result() for future in futures]
         else:
             cost = []
             for sc_gid, sc_table in groups:
-                capacity = cls._get_capacity(sc_gid, sc_table,
-                                             connectable=connectable,
-                                             sc_capacity_col=scc)
-                cost.append(TC.feature_costs(sc_table,
-                                             capacity=capacity,
-                                             avail_cap_frac=avail_cap_frac,
-                                             line_limited=line_limited,
-                                             **trans_costs))
+                capacity = cls._get_capacity(
+                    sc_gid,
+                    sc_table,
+                    connectable=connectable,
+                    sc_capacity_col=scc,
+                )
+                cost.append(
+                    TC.feature_costs(
+                        sc_table,
+                        capacity=capacity,
+                        avail_cap_frac=avail_cap_frac,
+                        line_limited=line_limited,
+                        **trans_costs,
+                    )
+                )
 
-        cost = np.hstack(cost).astype('float32')
-        logger.info('LCOT cost calculation is complete.')
+        cost = np.hstack(cost).astype("float32")
+        logger.info("LCOT cost calculation is complete.")
 
         return cost
 
-    def compute_total_lcoe(self, fcr, transmission_costs=None,
-                           avail_cap_frac=1, line_limited=False,
-                           connectable=True, max_workers=None,
-                           consider_friction=True):
+    def compute_total_lcoe(
+        self,
+        fcr,
+        transmission_costs=None,
+        avail_cap_frac=1,
+        line_limited=False,
+        connectable=True,
+        max_workers=None,
+        consider_friction=True,
+    ):
         """
         Compute LCOT and total LCOE for all sc point to transmission feature
         connections
 
         Parameters
         ----------
         fcr : float
@@ -824,70 +915,79 @@
         max_workers : int | NoneType, optional
             Number of workers to use to compute lcot, if > 1 run in parallel.
             None uses all available cpu's. by default None
         consider_friction : bool, optional
             Flag to consider friction layer on LCOE when "mean_lcoe_friction"
             is in the sc points input, by default True
         """
-        if 'trans_cap_cost' not in self._trans_table:
+        if "trans_cap_cost" not in self._trans_table:
             scc = self._sc_capacity_col
-            cost = self._compute_trans_cap_cost(self._trans_table,
-                                                trans_costs=transmission_costs,
-                                                avail_cap_frac=avail_cap_frac,
-                                                line_limited=line_limited,
-                                                connectable=connectable,
-                                                max_workers=max_workers,
-                                                sc_capacity_col=scc)
-            self._trans_table['trans_cap_cost_per_mw'] = cost  # $/MW
+            cost = self._compute_trans_cap_cost(
+                self._trans_table,
+                trans_costs=transmission_costs,
+                avail_cap_frac=avail_cap_frac,
+                line_limited=line_limited,
+                connectable=connectable,
+                max_workers=max_workers,
+                sc_capacity_col=scc,
+            )
+            self._trans_table["trans_cap_cost_per_mw"] = cost  # $/MW
         else:
-            cost = self._trans_table['trans_cap_cost'].values.copy()  # $
+            cost = self._trans_table["trans_cap_cost"].values.copy()  # $
             cost /= self._trans_table[self._sc_capacity_col]  # $/MW
-            self._trans_table['trans_cap_cost_per_mw'] = cost
+            self._trans_table["trans_cap_cost_per_mw"] = cost
 
         cost *= self._trans_table[self._sc_capacity_col]
-        cost /= self._trans_table['capacity']  # align with "mean_cf"
+        # align with "mean_cf"
+        cost /= self._trans_table[SupplyCurveField.CAPACITY]
 
         if 'reinforcement_cost_per_mw' in self._trans_table:
             logger.info("'reinforcement_cost_per_mw' column found in "
                         "transmission table. Adding reinforcement costs "
                         "to total LCOE.")
-            cf_mean_arr = self._trans_table['mean_cf'].values
+            cf_mean_arr = self._trans_table[SupplyCurveField.MEAN_CF].values
             lcot = (cost * fcr) / (cf_mean_arr * 8760)
-            lcoe = lcot + self._trans_table['mean_lcoe']
+            lcoe = lcot + self._trans_table[SupplyCurveField.MEAN_LCOE]
             self._trans_table['lcot_no_reinforcement'] = lcot
             self._trans_table['lcoe_no_reinforcement'] = lcoe
             r_cost = (self._trans_table['reinforcement_cost_per_mw']
                       .values.copy())
             r_cost *= self._trans_table[self._sc_capacity_col]
-            r_cost /= self._trans_table['capacity']  # align with "mean_cf"
+            # align with "mean_cf"
+            r_cost /= self._trans_table[SupplyCurveField.CAPACITY]
             cost += r_cost  # $/MW
 
-        cf_mean_arr = self._trans_table['mean_cf'].values
+        cf_mean_arr = self._trans_table[SupplyCurveField.MEAN_CF].values
         lcot = (cost * fcr) / (cf_mean_arr * 8760)
 
         self._trans_table['lcot'] = lcot
-        self._trans_table['total_lcoe'] = (self._trans_table['lcot']
-                                           + self._trans_table['mean_lcoe'])
+        self._trans_table['total_lcoe'] = (
+            self._trans_table['lcot']
+            + self._trans_table[SupplyCurveField.MEAN_LCOE])
 
         if consider_friction:
             self._calculate_total_lcoe_friction()
 
     def _calculate_total_lcoe_friction(self):
         """Look for site mean LCOE with friction in the trans table and if
         found make a total LCOE column with friction."""
 
-        if 'mean_lcoe_friction' in self._trans_table:
-            lcoe_friction = (self._trans_table['lcot']
-                             + self._trans_table['mean_lcoe_friction'])
-            self._trans_table['total_lcoe_friction'] = lcoe_friction
+        if SupplyCurveField.MEAN_LCOE_FRICTION in self._trans_table:
+            lcoe_friction = (
+                self._trans_table['lcot']
+                + self._trans_table[SupplyCurveField.MEAN_LCOE_FRICTION])
+            self._trans_table[SupplyCurveField.TOTAL_LCOE_FRICTION] = (
+                lcoe_friction
+            )
             logger.info('Found mean LCOE with friction. Adding key '
                         '"total_lcoe_friction" to trans table.')
 
-    def _exclude_noncompetitive_wind_farms(self, comp_wind_dirs, sc_gid,
-                                           downwind=False):
+    def _exclude_noncompetitive_wind_farms(
+        self, comp_wind_dirs, sc_gid, downwind=False
+    ):
         """
         Exclude non-competitive wind farms for given sc_gid
 
         Parameters
         ----------
         comp_wind_dirs : CompetitiveWindFarms
             Pre-initilized CompetitiveWindFarms instance
@@ -901,26 +1001,28 @@
         -------
         comp_wind_dirs : CompetitiveWindFarms
             updated CompetitiveWindFarms instance
         """
         gid = comp_wind_dirs.check_sc_gid(sc_gid)
         if gid is not None:
             if comp_wind_dirs.mask[gid]:
-                exclude_gids = comp_wind_dirs['upwind', gid]
+                exclude_gids = comp_wind_dirs["upwind", gid]
                 if downwind:
-                    exclude_gids = np.append(exclude_gids,
-                                             comp_wind_dirs['downwind', gid])
+                    exclude_gids = np.append(
+                        exclude_gids, comp_wind_dirs["downwind", gid]
+                    )
                 for n in exclude_gids:
                     check = comp_wind_dirs.exclude_sc_point_gid(n)
                     if check:
-                        sc_gids = comp_wind_dirs['sc_gid', n]
+                        sc_gids = comp_wind_dirs[SupplyCurveField.SC_GID, n]
                         for sc_id in sc_gids:
                             if self._mask[sc_id]:
-                                logger.debug('Excluding sc_gid {}'
-                                             .format(sc_id))
+                                logger.debug(
+                                    "Excluding sc_gid {}".format(sc_id)
+                                )
                                 self._mask[sc_id] = False
 
         return comp_wind_dirs
 
     @staticmethod
     def add_sum_cols(table, sum_cols):
         """Add a summation column to table.
@@ -941,34 +1043,49 @@
             Supply curve table with additional summation columns.
         """
 
         for new_label, sum_labels in sum_cols.items():
             missing = [s for s in sum_labels if s not in table]
 
             if any(missing):
-                logger.info('Could not make sum column "{}", missing: {}'
-                            .format(new_label, missing))
+                logger.info(
+                    'Could not make sum column "{}", missing: {}'.format(
+                        new_label, missing
+                    )
+                )
             else:
                 sum_arr = np.zeros(len(table))
                 for s in sum_labels:
                     temp = table[s].values
                     temp[np.isnan(temp)] = 0
                     sum_arr += temp
 
                 table[new_label] = sum_arr
 
         return table
 
-    def _full_sort(self, trans_table, trans_costs=None,
-                   avail_cap_frac=1, comp_wind_dirs=None,
-                   total_lcoe_fric=None, sort_on='total_lcoe',
-                   columns=('trans_gid', 'trans_capacity', 'trans_type',
-                            'trans_cap_cost_per_mw', 'dist_km', 'lcot',
-                            'total_lcoe'),
-                   downwind=False):
+    def _full_sort(
+        self,
+        trans_table,
+        trans_costs=None,
+        avail_cap_frac=1,
+        comp_wind_dirs=None,
+        total_lcoe_fric=None,
+        sort_on="total_lcoe",
+        columns=(
+            "trans_gid",
+            "trans_capacity",
+            "trans_type",
+            "trans_cap_cost_per_mw",
+            "dist_km",
+            "lcot",
+            "total_lcoe",
+        ),
+        downwind=False,
+    ):
         """
         Internal method to handle full supply curve sorting
 
         Parameters
         ----------
         trans_table : pandas.DataFrame
             Supply Curve Tranmission table to sort on
@@ -998,138 +1115,172 @@
 
         Returns
         -------
         supply_curve : pandas.DataFrame
             Updated sc_points table with transmission connections, LCOT
             and LCOE+LCOT based on full supply curve connections
         """
-        trans_features = self._create_handler(self._trans_table,
-                                              trans_costs=trans_costs,
-                                              avail_cap_frac=avail_cap_frac)
+        trans_features = self._create_handler(
+            self._trans_table,
+            trans_costs=trans_costs,
+            avail_cap_frac=avail_cap_frac,
+        )
         init_list = [np.nan] * int(1 + np.max(self._sc_gids))
         columns = list(columns)
         if sort_on not in columns:
             columns.append(sort_on)
 
         conn_lists = {k: deepcopy(init_list) for k in columns}
 
-        trans_sc_gids = trans_table['sc_gid'].values.astype(int)
+        trans_sc_gids = trans_table[SupplyCurveField.SC_GID].values.astype(int)
 
         # syntax is final_key: source_key (source from trans_table)
         all_cols = {k: k for k in columns}
-        essentials = {'trans_gid': 'trans_gid',
-                      'trans_capacity': 'avail_cap',
-                      'trans_type': 'category',
-                      'dist_km': 'dist_km',
-                      'trans_cap_cost_per_mw': 'trans_cap_cost_per_mw',
-                      'lcot': 'lcot',
-                      'total_lcoe': 'total_lcoe',
-                      }
+        essentials = {
+            "trans_gid": "trans_gid",
+            "trans_capacity": "avail_cap",
+            "trans_type": "category",
+            "dist_km": "dist_km",
+            "trans_cap_cost_per_mw": "trans_cap_cost_per_mw",
+            "lcot": "lcot",
+            "total_lcoe": "total_lcoe",
+        }
         all_cols.update(essentials)
 
-        arrays = {final_key: trans_table[source_key].values
-                  for final_key, source_key in all_cols.items()}
+        arrays = {
+            final_key: trans_table[source_key].values
+            for final_key, source_key in all_cols.items()
+        }
 
         sc_capacities = trans_table[self._sc_capacity_col].values
 
         connected = 0
         progress = 0
         for i in range(len(trans_table)):
             sc_gid = trans_sc_gids[i]
             if self._mask[sc_gid]:
-                connect = trans_features.connect(arrays['trans_gid'][i],
-                                                 sc_capacities[i])
+                connect = trans_features.connect(
+                    arrays["trans_gid"][i], sc_capacities[i]
+                )
                 if connect:
                     connected += 1
-                    logger.debug('Connecting sc gid {}'.format(sc_gid))
+                    logger.debug("Connecting sc gid {}".format(sc_gid))
                     self._mask[sc_gid] = False
 
                     for col_name, data_arr in arrays.items():
                         conn_lists[col_name][sc_gid] = data_arr[i]
 
                     if total_lcoe_fric is not None:
-                        conn_lists['total_lcoe_friction'][sc_gid] = \
-                            total_lcoe_fric[i]
+                        col_name = SupplyCurveField.TOTAL_LCOE_FRICTION
+                        conn_lists[col_name][sc_gid] = total_lcoe_fric[i]
 
                     current_prog = connected // (len(self) / 100)
                     if current_prog > progress:
                         progress = current_prog
-                        logger.info('{} % of supply curve points connected'
-                                    .format(progress))
+                        logger.info(
+                            "{} % of supply curve points connected".format(
+                                progress
+                            )
+                        )
 
                     if comp_wind_dirs is not None:
-                        comp_wind_dirs = \
+                        comp_wind_dirs = (
                             self._exclude_noncompetitive_wind_farms(
-                                comp_wind_dirs, sc_gid, downwind=downwind)
+                                comp_wind_dirs, sc_gid, downwind=downwind
+                            )
+                        )
 
         index = range(0, int(1 + np.max(self._sc_gids)))
         connections = pd.DataFrame(conn_lists, index=index)
-        connections.index.name = 'sc_gid'
+        connections.index.name = SupplyCurveField.SC_GID
         connections = connections.dropna(subset=[sort_on])
         connections = connections[columns].reset_index()
 
-        sc_gids = self._sc_points['sc_gid'].values
-        connected = connections['sc_gid'].values
+        sc_gids = self._sc_points[SupplyCurveField.SC_GID].values
+        connected = connections[SupplyCurveField.SC_GID].values
         logger.debug('Connected gids {} out of total supply curve gids {}'
                      .format(len(connected), len(sc_gids)))
         unconnected = ~np.isin(sc_gids, connected)
         unconnected = sc_gids[unconnected].tolist()
 
         if unconnected:
-            msg = ("{} supply curve points were not connected to tranmission! "
-                   "Unconnected sc_gid's: {}"
-                   .format(len(unconnected), unconnected))
+            msg = (
+                "{} supply curve points were not connected to tranmission! "
+                "Unconnected sc_gid's: {}".format(
+                    len(unconnected), unconnected
+                )
+            )
             logger.warning(msg)
             warn(msg)
 
-        supply_curve = self._sc_points.merge(connections, on='sc_gid')
+        supply_curve = self._sc_points.merge(
+            connections, on=SupplyCurveField.SC_GID)
 
         return supply_curve.reset_index(drop=True)
 
     def _check_feature_capacity(self, avail_cap_frac=1):
         """
         Add the transmission connection feature capacity to the trans table if
         needed
         """
-        if 'avail_cap' not in self._trans_table:
-            kwargs = {'avail_cap_frac': avail_cap_frac}
+        if "avail_cap" not in self._trans_table:
+            kwargs = {"avail_cap_frac": avail_cap_frac}
             fc = TF.feature_capacity(self._trans_table, **kwargs)
-            self._trans_table = self._trans_table.merge(fc, on='trans_gid')
+            self._trans_table = self._trans_table.merge(fc, on="trans_gid")
 
     def _adjust_output_columns(self, columns, consider_friction):
-        """Add extra output columns, if needed. """
+        """Add extra output columns, if needed."""
         # These are essentially should-be-defaults that are not
         # backwards-compatible, so have to explicitly check for them
         extra_cols = ['ba_str', 'poi_lat', 'poi_lon', 'reinforcement_poi_lat',
-                      'reinforcement_poi_lon', 'eos_mult', 'reg_mult',
+                      'reinforcement_poi_lon', SupplyCurveField.EOS_MULT,
+                      SupplyCurveField.REG_MULT,
                       'reinforcement_cost_per_mw', 'reinforcement_dist_km',
-                      'n_parallel_trans', 'total_lcoe_friction']
+                      'n_parallel_trans', SupplyCurveField.TOTAL_LCOE_FRICTION]
         if not consider_friction:
-            extra_cols -= {'total_lcoe_friction'}
+            extra_cols -= {SupplyCurveField.TOTAL_LCOE_FRICTION}
 
-        extra_cols = [col for col in extra_cols
-                      if col in self._trans_table and col not in columns]
+        extra_cols = [
+            col
+            for col in extra_cols
+            if col in self._trans_table and col not in columns
+        ]
 
         return columns + extra_cols
 
     def _determine_sort_on(self, sort_on):
         """Determine the `sort_on` column from user input and trans table"""
-        if 'reinforcement_cost_per_mw' in self._trans_table:
+        if "reinforcement_cost_per_mw" in self._trans_table:
             sort_on = sort_on or "lcoe_no_reinforcement"
-        return sort_on or 'total_lcoe'
+        return sort_on or "total_lcoe"
 
-    def full_sort(self, fcr, transmission_costs=None,
-                  avail_cap_frac=1, line_limited=False,
-                  connectable=True, max_workers=None,
-                  consider_friction=True, sort_on=None,
-                  columns=('trans_gid', 'trans_capacity', 'trans_type',
-                           'trans_cap_cost_per_mw', 'dist_km', 'lcot',
-                           'total_lcoe'),
-                  wind_dirs=None, n_dirs=2, downwind=False,
-                  offshore_compete=False):
+    def full_sort(
+        self,
+        fcr,
+        transmission_costs=None,
+        avail_cap_frac=1,
+        line_limited=False,
+        connectable=True,
+        max_workers=None,
+        consider_friction=True,
+        sort_on=None,
+        columns=(
+            "trans_gid",
+            "trans_capacity",
+            "trans_type",
+            "trans_cap_cost_per_mw",
+            "dist_km",
+            "lcot",
+            "total_lcoe",
+        ),
+        wind_dirs=None,
+        n_dirs=2,
+        downwind=False,
+        offshore_compete=False,
+    ):
         """
         run full supply curve sorting
 
         Parameters
         ----------
         fcr : float
             Fixed charge rate, used to compute LCOT
@@ -1176,72 +1327,96 @@
 
         Returns
         -------
         supply_curve : pandas.DataFrame
             Updated sc_points table with transmission connections, LCOT
             and LCOE+LCOT based on full supply curve connections
         """
-        logger.info('Starting full competitive supply curve sort.')
+        logger.info("Starting full competitive supply curve sort.")
         self._check_substation_conns(self._trans_table)
-        self.compute_total_lcoe(fcr, transmission_costs=transmission_costs,
-                                avail_cap_frac=avail_cap_frac,
-                                line_limited=line_limited,
-                                connectable=connectable,
-                                max_workers=max_workers,
-                                consider_friction=consider_friction)
+        self.compute_total_lcoe(
+            fcr,
+            transmission_costs=transmission_costs,
+            avail_cap_frac=avail_cap_frac,
+            line_limited=line_limited,
+            connectable=connectable,
+            max_workers=max_workers,
+            consider_friction=consider_friction,
+        )
         self._check_feature_capacity(avail_cap_frac=avail_cap_frac)
 
         if isinstance(columns, tuple):
             columns = list(columns)
 
         columns = self._adjust_output_columns(columns, consider_friction)
         sort_on = self._determine_sort_on(sort_on)
 
         trans_table = self._trans_table.copy()
-        pos = trans_table['lcot'].isnull()
-        trans_table = trans_table.loc[~pos].sort_values([sort_on, 'trans_gid'])
+        pos = trans_table["lcot"].isnull()
+        trans_table = trans_table.loc[~pos].sort_values([sort_on, "trans_gid"])
 
         total_lcoe_fric = None
-        if consider_friction and 'mean_lcoe_friction' in trans_table:
-            total_lcoe_fric = trans_table['total_lcoe_friction'].values
+        col_in_table = SupplyCurveField.MEAN_LCOE_FRICTION in trans_table
+        if consider_friction and col_in_table:
+            total_lcoe_fric = \
+                trans_table[SupplyCurveField.TOTAL_LCOE_FRICTION].values
 
         comp_wind_dirs = None
         if wind_dirs is not None:
             msg = "Excluding {} upwind".format(n_dirs)
             if downwind:
                 msg += " and downwind"
 
             msg += " onshore"
             if offshore_compete:
                 msg += " and offshore"
 
             msg += " windfarms"
             logger.info(msg)
-            comp_wind_dirs = CompetitiveWindFarms(wind_dirs,
-                                                  self._sc_points,
-                                                  n_dirs=n_dirs,
-                                                  offshore=offshore_compete)
-
-        supply_curve = self._full_sort(trans_table,
-                                       trans_costs=transmission_costs,
-                                       avail_cap_frac=avail_cap_frac,
-                                       comp_wind_dirs=comp_wind_dirs,
-                                       total_lcoe_fric=total_lcoe_fric,
-                                       sort_on=sort_on, columns=columns,
-                                       downwind=downwind)
+            comp_wind_dirs = CompetitiveWindFarms(
+                wind_dirs,
+                self._sc_points,
+                n_dirs=n_dirs,
+                offshore=offshore_compete,
+            )
+
+        supply_curve = self._full_sort(
+            trans_table,
+            trans_costs=transmission_costs,
+            avail_cap_frac=avail_cap_frac,
+            comp_wind_dirs=comp_wind_dirs,
+            total_lcoe_fric=total_lcoe_fric,
+            sort_on=sort_on,
+            columns=columns,
+            downwind=downwind,
+        )
 
         return supply_curve
 
-    def simple_sort(self, fcr, transmission_costs=None,
-                    avail_cap_frac=1, max_workers=None,
-                    consider_friction=True, sort_on=None,
-                    columns=('trans_gid', 'trans_type', 'lcot', 'total_lcoe',
-                             'dist_km', 'trans_cap_cost_per_mw'),
-                    wind_dirs=None, n_dirs=2, downwind=False,
-                    offshore_compete=False):
+    def simple_sort(
+        self,
+        fcr,
+        transmission_costs=None,
+        avail_cap_frac=1,
+        max_workers=None,
+        consider_friction=True,
+        sort_on=None,
+        columns=(
+            "trans_gid",
+            "trans_type",
+            "lcot",
+            "total_lcoe",
+            "dist_km",
+            "trans_cap_cost_per_mw",
+        ),
+        wind_dirs=None,
+        n_dirs=2,
+        downwind=False,
+        offshore_compete=False,
+    ):
         """
         Run simple supply curve sorting that does not take into account
         available capacity
 
         Parameters
         ----------
         fcr : float
@@ -1288,55 +1463,75 @@
 
         Returns
         -------
         supply_curve : pandas.DataFrame
             Updated sc_points table with transmission connections, LCOT
             and LCOE+LCOT based on simple supply curve connections
         """
-        logger.info('Starting simple supply curve sort (no capacity limits).')
-        self.compute_total_lcoe(fcr, transmission_costs=transmission_costs,
-                                avail_cap_frac=avail_cap_frac,
-                                connectable=False,
-                                max_workers=max_workers,
-                                consider_friction=consider_friction)
+        logger.info("Starting simple supply curve sort (no capacity limits).")
+        self.compute_total_lcoe(
+            fcr,
+            transmission_costs=transmission_costs,
+            avail_cap_frac=avail_cap_frac,
+            connectable=False,
+            max_workers=max_workers,
+            consider_friction=consider_friction,
+        )
         trans_table = self._trans_table.copy()
 
         if isinstance(columns, tuple):
             columns = list(columns)
 
         columns = self._adjust_output_columns(columns, consider_friction)
         sort_on = self._determine_sort_on(sort_on)
 
         connections = trans_table.sort_values([sort_on, 'trans_gid'])
-        connections = connections.groupby('sc_gid').first()
+        connections = connections.groupby(SupplyCurveField.SC_GID).first()
         rename = {'trans_gid': 'trans_gid',
                   'category': 'trans_type'}
         connections = connections.rename(columns=rename)
         connections = connections[columns].reset_index()
 
-        supply_curve = self._sc_points.merge(connections, on='sc_gid')
+        supply_curve = self._sc_points.merge(connections,
+                                             on=SupplyCurveField.SC_GID)
         if wind_dirs is not None:
-            supply_curve = \
-                CompetitiveWindFarms.run(wind_dirs,
-                                         supply_curve,
-                                         n_dirs=n_dirs,
-                                         offshore=offshore_compete,
-                                         sort_on=sort_on,
-                                         downwind=downwind)
+            supply_curve = CompetitiveWindFarms.run(
+                wind_dirs,
+                supply_curve,
+                n_dirs=n_dirs,
+                offshore=offshore_compete,
+                sort_on=sort_on,
+                downwind=downwind,
+            )
 
         supply_curve = supply_curve.reset_index(drop=True)
 
         return supply_curve
 
-    def run(self, out_fpath, fixed_charge_rate, simple=True, avail_cap_frac=1,
-            line_limited=False, transmission_costs=None,
-            consider_friction=True, sort_on=None,
-            columns=('trans_gid', 'trans_type', 'trans_cap_cost_per_mw',
-                     'dist_km', 'lcot', 'total_lcoe'),
-            max_workers=None, competition=None):
+    def run(
+        self,
+        out_fpath,
+        fixed_charge_rate,
+        simple=True,
+        avail_cap_frac=1,
+        line_limited=False,
+        transmission_costs=None,
+        consider_friction=True,
+        sort_on=None,
+        columns=(
+            "trans_gid",
+            "trans_type",
+            "trans_cap_cost_per_mw",
+            "dist_km",
+            "lcot",
+            "total_lcoe",
+        ),
+        max_workers=None,
+        competition=None,
+    ):
         """Run Supply Curve Transmission calculations.
 
         Run full supply curve taking into account available capacity of
         tranmission features when making connections.
 
         Parameters
         ----------
@@ -1429,20 +1624,22 @@
             By default ``None``.
 
         Returns
         -------
         str
             Path to output supply curve.
         """
-        kwargs = {"fcr": fixed_charge_rate,
-                  "transmission_costs": transmission_costs,
-                  "consider_friction": consider_friction,
-                  "sort_on": sort_on,
-                  "columns": columns,
-                  "max_workers": max_workers}
+        kwargs = {
+            "fcr": fixed_charge_rate,
+            "transmission_costs": transmission_costs,
+            "consider_friction": consider_friction,
+            "sort_on": sort_on,
+            "columns": columns,
+            "max_workers": max_workers,
+        }
         kwargs.update(competition or {})
 
         if simple:
             supply_curve = self.simple_sort(**kwargs)
         else:
             kwargs["avail_cap_frac"] = avail_cap_frac
             kwargs["line_limited"] = line_limited
@@ -1453,12 +1650,12 @@
 
         return out_fpath
 
 
 def _format_sc_out_fpath(out_fpath):
     """Add CSV file ending and replace underscore, if necessary."""
     if not out_fpath.endswith(".csv"):
-        out_fpath = '{}.csv'.format(out_fpath)
+        out_fpath = "{}.csv".format(out_fpath)
 
     project_dir, out_fn = os.path.split(out_fpath)
     out_fn = out_fn.replace("supply_curve", "supply-curve")
     return os.path.join(project_dir, out_fn)
```

### Comparing `NREL-reV-0.8.7/reV/supply_curve/tech_mapping.py` & `NREL-reV-0.8.9/reV/supply_curve/tech_mapping.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 This module manages the exclusions-to-resource mapping.
 The core of this module is a parallel cKDTree.
 
 Created on Fri Jun 21 16:05:47 2019
 
 @author: gbuster
 """
-from concurrent.futures import as_completed
-import h5py
 import logging
-from math import ceil
-import numpy as np
 import os
-from scipy.spatial import cKDTree
+from concurrent.futures import as_completed
+from math import ceil
 from warnings import warn
 
-from reV.supply_curve.extent import SupplyCurveExtent
-from reV.utilities.exceptions import FileInputWarning, FileInputError
-
+import h5py
+import numpy as np
 from rex.resource import Resource
 from rex.utilities.execution import SpawnProcessPool
 from rex.utilities.utilities import res_dist_threshold
+from scipy.spatial import cKDTree
+
+from reV.supply_curve.extent import SupplyCurveExtent, LATITUDE, LONGITUDE
+from reV.utilities.exceptions import FileInputError, FileInputWarning
 
 logger = logging.getLogger(__name__)
 
 
 class TechMapping:
     """Framework to create map between tech layer (exclusions), res, and gen"""
 
-    def __init__(self, excl_fpath, res_fpath, sc_resolution=2560,
-                 dist_margin=1.05):
+    def __init__(
+        self, excl_fpath, res_fpath, sc_resolution=2560, dist_margin=1.05
+    ):
         """
         Parameters
         ----------
         excl_fpath : str
             Filepath to exclusions h5 file, must contain latitude and longitude
             arrays to allow for mapping to resource points
         res_fpath : str
@@ -47,30 +48,35 @@
         dist_margin : float, optional
             Extra margin to multiply times the computed distance between
             neighboring resource points, by default 1.05
         """
         self._excl_fpath = excl_fpath
         self._check_fout()
 
-        self._tree, self._dist_thresh = \
-            self._build_tree(res_fpath, dist_margin=dist_margin)
-
-        with SupplyCurveExtent(self._excl_fpath,
-                               resolution=sc_resolution) as sc:
+        self._tree, self._dist_thresh = self._build_tree(
+            res_fpath, dist_margin=dist_margin
+        )
+
+        with SupplyCurveExtent(
+            self._excl_fpath, resolution=sc_resolution
+        ) as sc:
             self._sc_resolution = sc.resolution
             self._gids = np.array(list(range(len(sc))), dtype=np.uint32)
             self._excl_shape = sc.exclusions.shape
             self._n_excl = np.product(self._excl_shape)
             self._sc_row_indices = sc.row_indices
             self._sc_col_indices = sc.col_indices
             self._excl_row_slices = sc.excl_row_slices
             self._excl_col_slices = sc.excl_col_slices
-            logger.info('Initialized TechMapping object with {} calc chunks '
-                        'for {} tech exclusion points'
-                        .format(len(self._gids), self._n_excl))
+            logger.info(
+                "Initialized TechMapping object with {} calc chunks "
+                "for {} tech exclusion points".format(
+                    len(self._gids), self._n_excl
+                )
+            )
 
     @property
     def distance_threshold(self):
         """Get the upper bound on NN distance between excl and res points.
 
         Returns
         -------
@@ -106,16 +112,17 @@
         """
         with Resource(res_fpath) as f:
             lat_lons = f.lat_lon
 
         # pylint: disable=not-callable
         tree = cKDTree(lat_lons)
 
-        dist_thresh = res_dist_threshold(lat_lons, tree=tree,
-                                         margin=dist_margin)
+        dist_thresh = res_dist_threshold(
+            lat_lons, tree=tree, margin=dist_margin
+        )
 
         return tree, dist_thresh
 
     @staticmethod
     def _make_excl_iarr(shape):
         """
         Create 2D array of 1D index values for the flattened h5 excl extent
@@ -131,16 +138,17 @@
             2D array of 1D index values for the flattened h5 excl extent
         """
         iarr = np.arange(np.product(shape), dtype=np.uint32)
 
         return iarr.reshape(shape)
 
     @staticmethod
-    def _get_excl_slices(gid, sc_row_indices, sc_col_indices, excl_row_slices,
-                         excl_col_slices):
+    def _get_excl_slices(
+        gid, sc_row_indices, sc_col_indices, excl_row_slices, excl_col_slices
+    ):
         """
         Get the row and column slices of the exclusions grid corresponding
         to the supply curve point gid.
 
         Parameters
         ----------
         gid : int
@@ -171,15 +179,15 @@
         col_slice = excl_col_slices[sc_col_indices[gid]]
 
         return row_slice, col_slice
 
     @classmethod
     def _get_excl_coords(cls, excl_fpath, gids, sc_row_indices, sc_col_indices,
                          excl_row_slices, excl_col_slices,
-                         coord_labels=('latitude', 'longitude')):
+                         coord_labels=(LATITUDE, LONGITUDE)):
         """
         Extract the exclusion coordinates for teh desired gids for TechMapping.
 
         Parameters
         ----------
         gids : np.ndarray
             Supply curve gids with tech exclusion points to map to the
@@ -206,40 +214,52 @@
         Returns
         -------
         coords_out : list
             List of arrays of the un-projected latitude, longitude array of
             tech exclusion points. List entries correspond to input gids.
         """
         coords_out = []
-        with h5py.File(excl_fpath, 'r') as f:
+        with h5py.File(excl_fpath, "r") as f:
             for gid in gids:
-                row_slice, col_slice = cls._get_excl_slices(gid,
-                                                            sc_row_indices,
-                                                            sc_col_indices,
-                                                            excl_row_slices,
-                                                            excl_col_slices)
+                row_slice, col_slice = cls._get_excl_slices(
+                    gid,
+                    sc_row_indices,
+                    sc_col_indices,
+                    excl_row_slices,
+                    excl_col_slices,
+                )
                 try:
                     lats = f[coord_labels[0]][row_slice, col_slice]
                     lons = f[coord_labels[1]][row_slice, col_slice]
                     emeta = np.vstack((lats.flatten(), lons.flatten())).T
                 except Exception as e:
-                    m = ('Could not unpack coordinates for gid {} with '
-                         'row/col slice {}/{}. Received the following '
-                         'error:\n{}'.format(gid, row_slice, col_slice, e))
+                    m = (
+                        "Could not unpack coordinates for gid {} with "
+                        "row/col slice {}/{}. Received the following "
+                        "error:\n{}".format(gid, row_slice, col_slice, e)
+                    )
                     logger.error(m)
                     raise e
 
                 coords_out.append(emeta)
 
         return coords_out
 
     @classmethod
-    def map_resource_gids(cls, gids, excl_fpath, sc_row_indices,
-                          sc_col_indices, excl_row_slices, excl_col_slices,
-                          tree, dist_thresh):
+    def map_resource_gids(
+        cls,
+        gids,
+        excl_fpath,
+        sc_row_indices,
+        sc_col_indices,
+        excl_row_slices,
+        excl_col_slices,
+        tree,
+        dist_thresh,
+    ):
         """Map exclusion gids to the resource meta.
 
         Parameters
         ----------
         gids : np.ndarray
             Supply curve gids with tech exclusion points to map to the
             resource meta points.
@@ -268,33 +288,50 @@
 
         Returns
         -------
         ind : list
             List of arrays of index values from the NN. List entries correspond
             to input gids.
         """
-        logger.debug('Getting tech map coordinates for chunks {} through {}'
-                     .format(gids[0], gids[-1]))
+        logger.debug(
+            "Getting tech map coordinates for chunks {} through {}".format(
+                gids[0], gids[-1]
+            )
+        )
         ind_out = []
-        coords_out = cls._get_excl_coords(excl_fpath, gids, sc_row_indices,
-                                          sc_col_indices, excl_row_slices,
-                                          excl_col_slices)
-
-        logger.debug('Running tech mapping for chunks {} through {}'
-                     .format(gids[0], gids[-1]))
+        coords_out = cls._get_excl_coords(
+            excl_fpath,
+            gids,
+            sc_row_indices,
+            sc_col_indices,
+            excl_row_slices,
+            excl_col_slices,
+        )
+
+        logger.debug(
+            "Running tech mapping for chunks {} through {}".format(
+                gids[0], gids[-1]
+            )
+        )
         for i, _ in enumerate(gids):
             dist, ind = tree.query(coords_out[i])
             ind[(dist >= dist_thresh)] = -1
             ind_out.append(ind)
 
         return ind_out
 
     @staticmethod
-    def save_tech_map(excl_fpath, dset, indices, distance_threshold=None,
-                      res_fpath=None, chunks=(128, 128)):
+    def save_tech_map(
+        excl_fpath,
+        dset,
+        indices,
+        distance_threshold=None,
+        res_fpath=None,
+        chunks=(128, 128),
+    ):
         """Save tech mapping indices and coordinates to an h5 output file.
 
         Parameters
         ----------
         excl_fpath : str
             Filepath to exclusions h5 file to add techmap to as 'dset'
         dset : str
@@ -311,39 +348,48 @@
             Chunk shape of the 2D output datasets.
         """
         logger.info('Writing tech map "{}" to {}'.format(dset, excl_fpath))
 
         shape = indices.shape
         chunks = (np.min((shape[0], chunks[0])), np.min((shape[1], chunks[1])))
 
-        with h5py.File(excl_fpath, 'a') as f:
+        with h5py.File(excl_fpath, "a") as f:
             if dset in list(f):
-                wmsg = ('TechMap results dataset "{}" is being replaced '
-                        'in pre-existing Exclusions TechMapping file "{}"'
-                        .format(dset, excl_fpath))
+                wmsg = (
+                    'TechMap results dataset "{}" is being replaced '
+                    'in pre-existing Exclusions TechMapping file "{}"'.format(
+                        dset, excl_fpath
+                    )
+                )
                 logger.warning(wmsg)
                 warn(wmsg, FileInputWarning)
                 f[dset][...] = indices
             else:
-                f.create_dataset(dset, shape=shape, dtype=indices.dtype,
-                                 data=indices, chunks=chunks)
+                f.create_dataset(
+                    dset,
+                    shape=shape,
+                    dtype=indices.dtype,
+                    data=indices,
+                    chunks=chunks,
+                )
 
             if distance_threshold:
-                f[dset].attrs['distance_threshold'] = distance_threshold
+                f[dset].attrs["distance_threshold"] = distance_threshold
 
             if res_fpath:
-                f[dset].attrs['src_res_fpath'] = res_fpath
+                f[dset].attrs["src_res_fpath"] = res_fpath
 
-        logger.info('Successfully saved tech map "{}" to {}'
-                    .format(dset, excl_fpath))
+        logger.info(
+            'Successfully saved tech map "{}" to {}'.format(dset, excl_fpath)
+        )
 
     def _check_fout(self):
         """Check the TechMapping output file for cached data."""
         with h5py.File(self._excl_fpath, 'r') as f:
-            if 'latitude' not in f or 'longitude' not in f:
+            if LATITUDE not in f or LONGITUDE not in f:
                 emsg = ('Datasets "latitude" and/or "longitude" not in '
                         'pre-existing Exclusions TechMapping file "{}". '
                         'Cannot proceed.'
                         .format(os.path.basename(self._excl_fpath)))
                 logger.exception(emsg)
                 raise FileInputError(emsg)
 
@@ -366,62 +412,74 @@
             Index values of the NN resource point. -1 if no res point found.
             2D integer array with shape equal to the exclusions extent shape.
         """
         gid_chunks = ceil(len(self._gids) / points_per_worker)
         gid_chunks = np.array_split(self._gids, gid_chunks)
 
         # init full output arrays
-        indices = -1 * np.ones((self._n_excl, ), dtype=np.int32)
+        indices = -1 * np.ones((self._n_excl,), dtype=np.int32)
         iarr = self._make_excl_iarr(self._excl_shape)
 
         futures = {}
-        loggers = [__name__, 'reV']
-        with SpawnProcessPool(max_workers=max_workers,
-                              loggers=loggers) as exe:
-
+        loggers = [__name__, "reV"]
+        with SpawnProcessPool(max_workers=max_workers, loggers=loggers) as exe:
             # iterate through split executions, submitting each to worker
             for i, gid_set in enumerate(gid_chunks):
                 # submit executions and append to futures list
-                futures[exe.submit(self.map_resource_gids,
-                                   gid_set,
-                                   self._excl_fpath,
-                                   self._sc_row_indices,
-                                   self._sc_col_indices,
-                                   self._excl_row_slices,
-                                   self._excl_col_slices,
-                                   self._tree,
-                                   self.distance_threshold)] = i
+                futures[
+                    exe.submit(
+                        self.map_resource_gids,
+                        gid_set,
+                        self._excl_fpath,
+                        self._sc_row_indices,
+                        self._sc_col_indices,
+                        self._excl_row_slices,
+                        self._excl_col_slices,
+                        self._tree,
+                        self.distance_threshold,
+                    )
+                ] = i
 
             n_finished = 0
             for future in as_completed(futures):
                 n_finished += 1
-                logger.info('Parallel TechMapping futures collected: '
-                            '{} out of {}'
-                            .format(n_finished, len(futures)))
+                logger.info(
+                    "Parallel TechMapping futures collected: "
+                    "{} out of {}".format(n_finished, len(futures))
+                )
 
                 i = futures[future]
                 result = future.result()
 
                 for j, gid in enumerate(gid_chunks[i]):
                     row_slice, col_slice = self._get_excl_slices(
                         gid,
                         self._sc_row_indices,
                         self._sc_col_indices,
                         self._excl_row_slices,
-                        self._excl_col_slices)
+                        self._excl_col_slices,
+                    )
                     ind_slice = iarr[row_slice, col_slice].flatten()
                     indices[ind_slice] = result[j]
 
         indices = indices.reshape(self._excl_shape)
 
         return indices
 
     @classmethod
-    def run(cls, excl_fpath, res_fpath, dset=None, sc_resolution=2560,
-            dist_margin=1.05, max_workers=None, points_per_worker=10):
+    def run(
+        cls,
+        excl_fpath,
+        res_fpath,
+        dset=None,
+        sc_resolution=2560,
+        dist_margin=1.05,
+        max_workers=None,
+        points_per_worker=10,
+    ):
         """Run parallel mapping and save to h5 file.
 
         Parameters
         ----------
         excl_fpath : str
             Filepath to exclusions h5 (tech layer). dset will be
             created in excl_fpath.
@@ -446,19 +504,23 @@
 
         Returns
         -------
         indices : np.ndarray
             Index values of the NN resource point. -1 if no res point found.
             2D integer array with shape equal to the exclusions extent shape.
         """
-        kwargs = {"dist_margin": dist_margin,
-                  "sc_resolution": sc_resolution}
+        kwargs = {"dist_margin": dist_margin, "sc_resolution": sc_resolution}
         mapper = cls(excl_fpath, res_fpath, **kwargs)
-        indices = mapper.map_resource(max_workers=max_workers,
-                                      points_per_worker=points_per_worker)
+        indices = mapper.map_resource(
+            max_workers=max_workers, points_per_worker=points_per_worker
+        )
 
         if dset:
-            mapper.save_tech_map(excl_fpath, dset, indices,
-                                 distance_threshold=mapper.distance_threshold,
-                                 res_fpath=res_fpath)
+            mapper.save_tech_map(
+                excl_fpath,
+                dset,
+                indices,
+                distance_threshold=mapper.distance_threshold,
+                res_fpath=res_fpath,
+            )
 
         return indices
```

### Comparing `NREL-reV-0.8.7/reV/utilities/cli_functions.py` & `NREL-reV-0.8.9/reV/utilities/cli_functions.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/utilities/curtailment.py` & `NREL-reV-0.8.9/reV/utilities/curtailment.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/utilities/exceptions.py` & `NREL-reV-0.8.9/reV/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/reV/utilities/pytest_utils.py` & `NREL-reV-0.8.9/reV/utilities/pytest_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # -*- coding: utf-8 -*-
 """Functions used for pytests"""
 
-import numpy as np
 import os
+
+import numpy as np
 import pandas as pd
 from packaging import version
 from rex.outputs import Outputs as RexOutputs
 
+from reV.utilities import ResourceMetaField
+
 
 def pd_date_range(*args, **kwargs):
     """A simple wrapper on the pd.date_range() method that handles the closed
     vs. inclusive kwarg change in pd 1.4.0"""
     incl = version.parse(pd.__version__) >= version.parse('1.4.0')
 
     if incl and 'closed' in kwargs:
@@ -85,15 +88,16 @@
                           inclusive='left')
     s_slices = [slice(0, 25), slice(25, 50)]
     out_pattern = os.path.join(td, 'chunks_{i}_{j}.h5')
 
     for i, s1 in enumerate(s_slices):
         for j, s2 in enumerate(s_slices):
             out_file = out_pattern.format(i=i, j=j)
-            meta = pd.DataFrame({'latitude': lat[s1, s2].flatten(),
-                                 'longitude': lon[s1, s2].flatten(),
-                                 'gid': gids[s1, s2].flatten()})
+            meta = pd.DataFrame(
+                {ResourceMetaField.LATITUDE: lat[s1, s2].flatten(),
+                 ResourceMetaField.LONGITUDE: lon[s1, s2].flatten(),
+                 ResourceMetaField.GID: gids[s1, s2].flatten()})
             write_chunk(meta=meta, times=times, data=data[s1, s2],
                         features=features, out_file=out_file)
 
     out = (out_pattern.format(i='*', j='*'), data, features, s_slices, times)
     return out
```

### Comparing `NREL-reV-0.8.7/reV/utilities/slots.py` & `NREL-reV-0.8.9/reV/utilities/slots.py`

 * *Files identical despite different names*

### Comparing `NREL-reV-0.8.7/setup.py` & `NREL-reV-0.8.9/setup.py`

 * *Files identical despite different names*

