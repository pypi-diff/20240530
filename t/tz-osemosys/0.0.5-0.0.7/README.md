# Comparing `tmp/tz_osemosys-0.0.5.tar.gz` & `tmp/tz_osemosys-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tz_osemosys-0.0.5.tar", last modified: Wed May 22 11:17:51 2024, max compression
+gzip compressed data, was "tz_osemosys-0.0.7.tar", last modified: Thu May 30 15:11:04 2024, max compression
```

## Comparing `tz_osemosys-0.0.5.tar` & `tz_osemosys-0.0.7.tar`

### file list

```diff
@@ -1,630 +1,749 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.914734 tz_osemosys-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.818733 tz_osemosys-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.818733 tz_osemosys-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.818733 tz_osemosys-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/workflows/ci-test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.github/workflows/test_pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/CODE-OF-CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-22 11:17:51.914734 tz_osemosys-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.818733 tz_osemosys-0.0.5/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/bin/memory_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.822733 tz_osemosys-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/commodity.md
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/impact.md
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/model.md
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/operating_mode.md
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/region.md
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/storage.md
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/technology.md
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/time_definition.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/docs/tutorials.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.822733 tz_osemosys-0.0.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.822733 tz_osemosys-0.0.5/examples/CAISO-ERCOT-IC/
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/CAISO-ERCOT-IC/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/CAISO-ERCOT-IC/technologies.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.814733 tz_osemosys-0.0.5/examples/otoole_compat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.822733 tz_osemosys-0.0.5/examples/otoole_compat/config_files/
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/config_files/otoole-full-electricity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/config_files/otoole-simple-hydro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.814733 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.830733 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/AccumulatedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/AnnualEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/AnnualExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/AvailabilityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityOfOneTechnologyUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityToActivityUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    30527 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCostStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionld.csv
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionlh.csv
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionls.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DAILYTIMEBRACKET.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DAYTYPE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DaySplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DaysInDayType.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DepreciationMethod.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRateIdv.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRateStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/EMISSION.csv
--rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/FUEL.csv
--rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/FixedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/InputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/MODE_OF_OPERATION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/MinStorageCharge.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ModelPeriodEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ModelPeriodExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/OperationalLife.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/OperationalLifeStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/OutputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/REGION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/REMinProductionTarget.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/RETagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/RETagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMargin.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMarginTagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMarginTagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualStorageCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/SEASON.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/STORAGE.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedDemandProfile.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/StorageLevelStart.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/StorageMaxChargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/StorageMaxDischargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TECHNOLOGY.csv
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TIMESLICE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TechnologyFromStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TechnologyToStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMinCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMinCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyAnnualActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyAnnualActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TradeRoute.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/YEAR.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/YearSplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/_REGION.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.842733 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AccumulatedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AvailabilityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)    55323 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityOfOneTechnologyUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityToActivityUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53273 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCostStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionld.csv
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionlh.csv
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionls.csv
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DAILYTIMEBRACKET.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DAYTYPE.csv
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaySplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaysInDayType.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DepreciationMethod.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRateIdv.csv
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRateStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EMISSION.csv
--rw-r--r--   0 runner    (1001) docker     (127)   122456 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FUEL.csv
--rw-r--r--   0 runner    (1001) docker     (127)    51815 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FixedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)   127042 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/InputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MODE_OF_OPERATION.csv
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MinStorageCharge.csv
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ModelPeriodEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ModelPeriodExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLife.csv
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLifeStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)   203338 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OutputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REGION.csv
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REMinProductionTarget.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMargin.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualStorageCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SEASON.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/STORAGE.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedDemandProfile.csv
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageLevelStart.csv
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageMaxChargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageMaxDischargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TECHNOLOGY.csv
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TIMESLICE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TechnologyFromStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TechnologyToStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)    19511 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TradeRoute.csv
--rw-r--r--   0 runner    (1001) docker     (127)    82323 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YEAR.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YearSplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/_REGION.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.854733 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AccumulatedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AnnualEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AnnualExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AvailabilityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityOfOneTechnologyUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityToActivityUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCostStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionld.csv
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionlh.csv
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionls.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DAILYTIMEBRACKET.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DAYTYPE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaySplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaysInDayType.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DepreciationMethod.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRateIdv.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRateStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EMISSION.csv
--rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FUEL.csv
--rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FixedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/InputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/MODE_OF_OPERATION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/MinStorageCharge.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ModelPeriodEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ModelPeriodExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OperationalLife.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OperationalLifeStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)   117964 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OutputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/REGION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/REMinProductionTarget.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/RETagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/RETagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMargin.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMarginTagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMarginTagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualStorageCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SEASON.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/STORAGE.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedDemandProfile.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageLevelStart.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageMaxChargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageMaxDischargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TECHNOLOGY.csv
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TIMESLICE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TechnologyFromStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TechnologyToStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMinCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMinCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyAnnualActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyAnnualActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyModelPeriodActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyModelPeriodActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TradeRoute.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YEAR.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YearSplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/_REGION.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.866733 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AccumulatedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AnnualEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AnnualExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AvailabilityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityOfOneTechnologyUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityToActivityUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCostStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionld.csv
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionlh.csv
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionls.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DAILYTIMEBRACKET.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DAYTYPE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaySplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaysInDayType.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DepreciationMethod.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRateIdv.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRateStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EMISSION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FUEL.csv
--rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FixedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/InputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/MODE_OF_OPERATION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/MinStorageCharge.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ModelPeriodEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ModelPeriodExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OperationalLife.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OperationalLifeStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OutputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/REGION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/REMinProductionTarget.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/RETagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/RETagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMargin.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMarginTagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMarginTagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualStorageCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SEASON.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/STORAGE.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedDemandProfile.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageLevelStart.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageMaxChargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageMaxDischargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TECHNOLOGY.csv
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TIMESLICE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TechnologyFromStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TechnologyToStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMinCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMinCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyAnnualActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyAnnualActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyModelPeriodActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyModelPeriodActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TradeRoute.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YEAR.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YearSplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/_REGION.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.874733 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AccumulatedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AnnualEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AnnualExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AvailabilityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityOfOneTechnologyUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityToActivityUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCostStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionld.csv
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionlh.csv
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionls.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DAILYTIMEBRACKET.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DAYTYPE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaySplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaysInDayType.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DepreciationMethod.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRateIdv.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRateStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EMISSION.csv
--rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FUEL.csv
--rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FixedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    71503 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/InputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/MODE_OF_OPERATION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/MinStorageCharge.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ModelPeriodEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ModelPeriodExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OperationalLife.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OperationalLifeStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OutputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/REGION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/REMinProductionTarget.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/RETagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/RETagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMargin.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMarginTagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMarginTagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualStorageCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SEASON.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/STORAGE.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedDemandProfile.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageLevelStart.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageMaxChargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageMaxDischargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TECHNOLOGY.csv
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TIMESLICE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TechnologyFromStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TechnologyToStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMinCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMinCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyAnnualActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyAnnualActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyModelPeriodActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyModelPeriodActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TradeRoute.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YEAR.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YearSplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/_REGION.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.886733 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/AccumulatedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/AnnualEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/AnnualExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/AvailabilityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityFactor.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityOfOneTechnologyUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityToActivityUnit.csv
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCostStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionld.csv
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionlh.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionls.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DAILYTIMEBRACKET.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DAYTYPE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DaySplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DaysInDayType.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DepreciationMethod.csv
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRateIdv.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRateStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/EMISSION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/EmissionActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/EmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/FUEL.csv
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/FixedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/InputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/MODE_OF_OPERATION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/MinStorageCharge.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/ModelPeriodEmissionLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/ModelPeriodExogenousEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/OperationalLife.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/OperationalLifeStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/OutputActivityRatio.csv
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/REGION.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/REMinProductionTarget.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/RETagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/RETagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMargin.csv
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMarginTagFuel.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMarginTagTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/ResidualCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/ResidualStorageCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/SEASON.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/STORAGE.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedAnnualDemand.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedDemandProfile.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageLevelStart.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageMaxChargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageMaxDischargeRate.csv
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TECHNOLOGY.csv
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TIMESLICE.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TechnologyFromStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TechnologyToStorage.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMaxCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMaxCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMinCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMinCapacityInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyAnnualActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyAnnualActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivityLowerLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivityUpperLimit.csv
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/TradeRoute.csv
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/VariableCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/YEAR.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/YearSplit.csv
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/_REGION.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.814733 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.890733 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/
--rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AccumulatedNewCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualEmissions.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualFixedOperatingCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmissionByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualVariableOperatingCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/CapitalInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/Demand.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedSalvageValue.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedTechnologyEmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/NewCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)   209150 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)    26252 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnologyAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (127)   172779 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfActivity.csv
--rw-r--r--   0 runner    (1001) docker     (127)   205093 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)   213389 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnologyByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)   113730 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)   118340 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnologyByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/SalvageValue.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21669 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalAnnualTechnologyActivityByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20347 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalCapacityAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalDiscountedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20471 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyAnnualActivity.csv
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivity.csv
--rw-r--r--   0 runner    (1001) docker     (127)   115801 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/UseByTechnology.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.898733 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AccumulatedNewCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualEmissions.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualFixedOperatingCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualTechnologyEmission.csv
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualTechnologyEmissionByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualVariableOperatingCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/CapitalInvestment.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/Demand.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedSalvageValue.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedTechnologyEmissionsPenalty.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/NewCapacity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    48446 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnologyAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (127)    42760 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfActivity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    48459 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)    50925 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnologyByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnology.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33426 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnologyByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/SalvageValue.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalAnnualTechnologyActivityByMode.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalCapacityAnnual.csv
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalDiscountedCost.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyAnnualActivity.csv
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivity.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31767 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/UseByTechnology.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.898733 tz_osemosys-0.0.5/examples/quickstart/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/quickstart/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.898733 tz_osemosys-0.0.5/examples/utopia/
--rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/examples/utopia/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:17:51.914734 tz_osemosys-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.898733 tz_osemosys-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.898733 tz_osemosys-0.0.5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/fixtures/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/fixtures/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.898733 tz_osemosys-0.0.5/tests/test_compatability/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_runspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_compatability/test_otoole_timedef.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.898733 tz_osemosys-0.0.5/tests/test_composition/
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_composition/test_compose_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_composition/test_compose_runspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.902733 tz_osemosys-0.0.5/tests/test_construction/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_load_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_runspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_construction/test_timedefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.902733 tz_osemosys-0.0.5/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_integration/test_linopy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.902733 tz_osemosys-0.0.5/tests/test_solve/
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_solve/test_salvage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_solve/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tests/test_solve/test_to_xr_ds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.814733 tz_osemosys-0.0.5/tz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.902733 tz_osemosys-0.0.5/tz/osemosys/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.902733 tz_osemosys-0.0.5/tz/osemosys/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/io/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/io/simpleeval.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.902733 tz_osemosys-0.0.5/tz/osemosys/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.906733 tz_osemosys-0.0.5/tz/osemosys/model/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/_accounting_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/_capital_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/_operating_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/_salvage_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/_total_discounted_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/annual_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/capacity_adequacy_a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/capacity_adequacy_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/energy_balance_a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/energy_balance_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/new_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/re_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/reserve_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/total_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/constraints/total_capacity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.906733 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/discounting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/financials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/reserve_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.910734 tz_osemosys-0.0.5/tz/osemosys/model/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/variables/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/variables/capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/model/variables/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.910734 tz_osemosys-0.0.5/tz/osemosys/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/commodity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.910734 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/impact.py
--rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    19849 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/technology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/compat/time_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/impact.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15398 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/technology.py
--rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/time_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.914734 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/commodity_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/impact_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/model_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22164 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/model_presolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/region_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/storage_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/technology_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12528 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/timedefinition_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/schemas/validation/validation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.914734 tz_osemosys-0.0.5/tz/osemosys/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/utils/cfg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-22 11:17:45.000000 tz_osemosys-0.0.5/tz/osemosys/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:17:51.914734 tz_osemosys-0.0.5/tz_osemosys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-22 11:17:51.000000 tz_osemosys-0.0.5/tz_osemosys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    43183 2024-05-22 11:17:51.000000 tz_osemosys-0.0.5/tz_osemosys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:17:51.000000 tz_osemosys-0.0.5/tz_osemosys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 11:17:51.000000 tz_osemosys-0.0.5/tz_osemosys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-22 11:17:51.000000 tz_osemosys-0.0.5/tz_osemosys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.991823 tz_osemosys-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.863822 tz_osemosys-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.867822 tz_osemosys-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.867822 tz_osemosys-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/workflows/ci-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.github/workflows/test_pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-30 15:11:04.991823 tz_osemosys-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.867822 tz_osemosys-0.0.7/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/bin/memory_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.867822 tz_osemosys-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/commodity.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/impact.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/model.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/operating_mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/region.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/storage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/technology.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/time_definition.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/docs/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.867822 tz_osemosys-0.0.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.867822 tz_osemosys-0.0.7/examples/CAISO-ERCOT-IC/
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/CAISO-ERCOT-IC/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/CAISO-ERCOT-IC/technologies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.859822 tz_osemosys-0.0.7/examples/otoole_compat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.867822 tz_osemosys-0.0.7/examples/otoole_compat/config_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/config_files/otoole-full-electricity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/config_files/otoole-simple-hydro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.859822 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.879822 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30527 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.887822 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    55323 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53273 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   122456 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    51815 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   127042 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   203338 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    19511 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    82323 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.899823 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   117964 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.911823 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.923823 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    71503 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.931823 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityOfOneTechnologyUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.859822 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.935823 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AccumulatedNewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualEmissions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualFixedOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmissionByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualVariableOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/CapitalInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/Demand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedSalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedTechnologyEmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/NewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   209150 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    26252 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnologyAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   172779 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   205093 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   213389 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   113730 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   118340 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/SalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21669 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalAnnualTechnologyActivityByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20347 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalCapacityAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalDiscountedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20471 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyAnnualActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyModelPeriodActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   115801 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/UseByTechnology.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.943823 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AccumulatedNewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualEmissions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualFixedOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualTechnologyEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualTechnologyEmissionByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualVariableOperatingCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/CapitalInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/Demand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedSalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedTechnologyEmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/NewCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    48446 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnologyAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    42760 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    48459 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    50925 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33426 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnologyByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/SalvageValue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalAnnualTechnologyActivityByMode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalCapacityAnnual.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalDiscountedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyAnnualActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyModelPeriodActivity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31767 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/UseByTechnology.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.943823 tz_osemosys-0.0.7/examples/quickstart/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/quickstart/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.943823 tz_osemosys-0.0.7/examples/utopia/
+-rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/examples/utopia/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:11:04.991823 tz_osemosys-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.943823 tz_osemosys-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.943823 tz_osemosys-0.0.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/fixtures/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/fixtures/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.863822 tz_osemosys-0.0.7/tests/otoole_compare/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.951823 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)    61851 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    70130 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30644 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    73135 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   120055 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54999 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.971823 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/AccumulatedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/AnnualEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/AnnualExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/AvailabilityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    55323 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/CapacityFactor.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    55893 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/CapitalCostStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/Conversionld.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/Conversionlh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/Conversionls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DAILYTIMEBRACKET.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DAYTYPE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DaySplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DaysInDayType.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DepreciationMethod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DiscountRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DiscountRateIdv.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/DiscountRateStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   125108 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/EmissionActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/EmissionsPenalty.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53507 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   131122 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/MinStorageCharge.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/ModelPeriodEmissionLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/ModelPeriodExogenousEmission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/OperationalLifeStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   203338 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/REMinProductionTarget.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/RETagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/RETagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/ReserveMargin.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/ReserveMarginTagFuel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/ReserveMarginTagTechnology.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/ResidualCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/ResidualStorageCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/SEASON.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/StorageLevelStart.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/StorageMaxChargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/StorageMaxDischargeRate.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TechnologyFromStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TechnologyToStorage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    19715 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMaxCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMaxCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMinCapacity.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMinCapacityInvestment.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyAnnualActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyAnnualActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityLowerLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityUpperLimit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/TradeRoute.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    82731 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/VariableCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-full-electricity-complete/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.975823 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/CapacityToActivityUnit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/CapitalCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/EMISSION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/FUEL.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/FixedCost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/InputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/MODE_OF_OPERATION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/OperationalLife.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/OutputActivityRatio.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/REGION.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/STORAGE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/SpecifiedAnnualDemand.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/SpecifiedDemandProfile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/TECHNOLOGY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/TIMESLICE.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/YEAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/YearSplit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/otoole_compare/otoole-simple-hydro/_REGION.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.975823 tz_osemosys-0.0.7/tests/test_compatability/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_runspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_compatability/test_otoole_timedef.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.975823 tz_osemosys-0.0.7/tests/test_composition/
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_composition/test_compose_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_composition/test_compose_runspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.975823 tz_osemosys-0.0.7/tests/test_construction/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_load_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_runspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_construction/test_timedefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.975823 tz_osemosys-0.0.7/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_integration/test_linopy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.979823 tz_osemosys-0.0.7/tests/test_solve/
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_solve/test_growth_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_solve/test_salvage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_solve/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tests/test_solve/test_to_xr_ds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.863822 tz_osemosys-0.0.7/tz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.979823 tz_osemosys-0.0.7/tz/osemosys/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.979823 tz_osemosys-0.0.7/tz/osemosys/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/io/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/io/simpleeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.979823 tz_osemosys-0.0.7/tz/osemosys/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.983823 tz_osemosys-0.0.7/tz/osemosys/model/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/_accounting_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/_capital_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/_operating_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/_salvage_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/_total_discounted_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/annual_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/capacity_adequacy_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/capacity_adequacy_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/capacity_growth_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/energy_balance_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/energy_balance_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/new_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/re_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/reserve_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/total_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/constraints/total_capacity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.983823 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/discounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/financials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/reserve_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.983823 tz_osemosys-0.0.7/tz/osemosys/model/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/variables/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/variables/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/model/variables/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.987823 tz_osemosys-0.0.7/tz/osemosys/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17858 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/commodity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.987823 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/compat/time_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18005 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/time_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.991823 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/commodity_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/impact_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/model_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22164 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/model_presolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/region_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/storage_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/technology_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12528 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/timedefinition_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/schemas/validation/validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.991823 tz_osemosys-0.0.7/tz/osemosys/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/utils/cfg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-05-30 15:10:57.000000 tz_osemosys-0.0.7/tz/osemosys/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:11:04.991823 tz_osemosys-0.0.7/tz_osemosys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-30 15:11:04.000000 tz_osemosys-0.0.7/tz_osemosys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    51206 2024-05-30 15:11:04.000000 tz_osemosys-0.0.7/tz_osemosys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:11:04.000000 tz_osemosys-0.0.7/tz_osemosys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 15:11:04.000000 tz_osemosys-0.0.7/tz_osemosys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 15:11:04.000000 tz_osemosys-0.0.7/tz_osemosys.egg-info/top_level.txt
```

### Comparing `tz_osemosys-0.0.5/.github/ISSUE_TEMPLATE/bug_report.yaml` & `tz_osemosys-0.0.7/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/.github/ISSUE_TEMPLATE/feature_request.yaml` & `tz_osemosys-0.0.7/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/.github/release-drafter.yml` & `tz_osemosys-0.0.7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/.github/workflows/ci-test.yaml` & `tz_osemosys-0.0.7/.github/workflows/ci-test.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/.github/workflows/pypi_publish.yml` & `tz_osemosys-0.0.7/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/.github/workflows/test_pypi_publish.yml` & `tz_osemosys-0.0.7/.github/workflows/test_pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/.gitignore` & `tz_osemosys-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/.pre-commit-config.yaml` & `tz_osemosys-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/CODE-OF-CONDUCT.md` & `tz_osemosys-0.0.7/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/CONTRIBUTING.md` & `tz_osemosys-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/LICENSE` & `tz_osemosys-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/PKG-INFO` & `tz_osemosys-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tz-osemosys
-Version: 0.0.5
+Version: 0.0.7
 Summary: An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero
 Author-email: Lucas Kruitwagen <lucas.kruitwagen@gmail.com>, Ed Gill <edwardxtg@gmail.com>, Abhishek Shivakumar <abhishek0208@gmail.com>
 Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org
 Project-URL: Source, https://github.com/transitionzero/tz-osemosys
 Keywords: energy,milp,climate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.5 Summary: An OSeMOSYS
+Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.7 Summary: An OSeMOSYS
 implementation for the Future Energy Outlook by TransitionZero Author-email:
 Lucas Kruitwagen
 gmail.com>, Ed Gill
 gmail.com>, Abhishek Shivakumar
 gmail.com> Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org Project-URL: Source, https://
```

### Comparing `tz_osemosys-0.0.5/README.md` & `tz_osemosys-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/bin/memory_profile.py` & `tz_osemosys-0.0.7/bin/memory_profile.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/docs/commodity.md` & `tz_osemosys-0.0.7/docs/commodity.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 `demand_profile` `({region:{year:{timeslice:float}})` - OSeMOSYS SpecifiedDemandProfile.
 Specified for a demand which varies by
 timeslice. If `demand_annual` is given for a commodity but `demand_profile` is not, the demand
 is treated as having an accumulated demand, which must be met for each year within any
 combination of timeslices. Optional, defaults to `None`.
 
-`is_renewable` `({region:{year:bool}})` - OSeMOSYS RETagFuel.
+`include_in_joint_renewable_target` `({region:{year:bool}})` - OSeMOSYS RETagFuel.
 Boolean tag to mark commodities which are considered
 as renewable for applying renewable generation targets. Optional, defaults to `None`.
 
 
 
 ## Examples
```

### Comparing `tz_osemosys-0.0.5/docs/impact.md` & `tz_osemosys-0.0.7/docs/impact.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/docs/index.md` & `tz_osemosys-0.0.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/docs/model.md` & `tz_osemosys-0.0.7/docs/model.md`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 `reserve_margin` `({region:{year:float}})` - OSeMOSYS ReserveMargin.
 Minimum level of the reserve margin required to be provided for all the tagged commodities, by
 the tagged technologies. If no reserve margin is required, the parameter will have value 1; if,
 for instance, 20% reserve margin is required, the parameter will have value 1.2.
 Optional parameter, defaults to 1.
 
 `renewable_production_target` `({region:{year:float}})` - OSeMOSYS REMinProductionTarget.
-Minimum ratio of all renewable commodities tagged in the is_renewable parameter, to be
-produced by the technologies tagged with the is_renewable parameter.
+Minimum ratio of all renewable commodities tagged in the include_in_joint_renewable_target parameter, to be
+produced by the technologies tagged with the include_in_joint_renewable_target parameter.
 Optional parameter, defaults to `None`.
 
 ## Examples
 
 ### From dicts
 
 A simple example of how a Runspec object might be created directly from provided data is below:
```

### Comparing `tz_osemosys-0.0.5/docs/operating_mode.md` & `tz_osemosys-0.0.7/docs/operating_mode.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/docs/region.md` & `tz_osemosys-0.0.7/docs/region.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/docs/storage.md` & `tz_osemosys-0.0.7/docs/storage.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/docs/technology.md` & `tz_osemosys-0.0.7/docs/technology.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Optional, defaults to 1.
 
 `capacity_one_tech_unit` `({region:{year:float}})` - OSeMOSYS CapacityOfOneTechnologyUnit.
 Capacity of one new unit of a technology. In case the user sets this parameter, the related
 technology will be installed only in batches of the specified capacity and the problem will
 turn into a Mixed Integer Linear Problem. Optional, defaults to `None`.
 
-`is_renewable` `({region:{year:bool}})` - OSeMOSYS RETagTechnology.
+`include_in_joint_renewable_target` `({region:{year:bool}})` - OSeMOSYS RETagTechnology.
 Boolean tagging the renewable technologies that must contribute to reaching the indicated
 minimum renewable production target. It has value True for thetechnologies contributing,
 False otherwise. Optional, defaults to `None`.
 
 `capacity_gross_max` `({region:{year:float}})` - OSeMOSYS TotalAnnualMaxCapacity.
 Total maximum existing (residual plus cumulatively installed) capacity allowed for a technology
 in a specified year. Optional, defaults to `None`.
```

### Comparing `tz_osemosys-0.0.5/docs/time_definition.md` & `tz_osemosys-0.0.7/docs/time_definition.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/CAISO-ERCOT-IC/main.yaml` & `tz_osemosys-0.0.7/examples/CAISO-ERCOT-IC/main.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 #     long_name: solar photovoltaic
 #     description: solar photovoltaic
 #     activity_unit_ratio: 30.41667
 #     capacity_addition_size: null
 #     availability_factor: 1.
 #     capacity_factor: 1.
 #     operating_life: 25
-#     is_renewable: true
+#     include_in_joint_renewable_target: true
 #     include_regions: null
 #     exclude_regions:
 #       - ATLANTIC-MARKET
 #       - PACIFIC-MARKET
 #     capex:
 #       "*": "{y:700 - 100*(max(${time_definition.years})-y)/(max(${time_definition.years}) - min(${time_definition.years})) for y in ${time_definition.years}}"
 #     opex_fixed: 10
```

### Comparing `tz_osemosys-0.0.5/examples/CAISO-ERCOT-IC/technologies.yaml` & `tz_osemosys-0.0.7/examples/CAISO-ERCOT-IC/technologies.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/README.md` & `tz_osemosys-0.0.7/examples/README.md`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/config_files/otoole-full-electricity.yaml` & `tz_osemosys-0.0.7/examples/otoole_compat/config_files/otoole-full-electricity.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/config_files/otoole-simple-hydro.yaml` & `tz_osemosys-0.0.7/examples/otoole_compat/config_files/otoole-simple-hydro.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityFactor.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityFactor.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityToActivityUnit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapacityToActivityUnit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/CapitalCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/DaysInDayType.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/DaysInDayType.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionsPenalty.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/EmissionsPenalty.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/FixedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/FixedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/InputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/InputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/OutputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/OutputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/ResidualCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedAnnualDemand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedAnnualDemand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedDemandProfile.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/SpecifiedDemandProfile.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TECHNOLOGY.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TECHNOLOGY.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacityInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/TotalAnnualMaxCapacityInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/VariableCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/VariableCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity/YearSplit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity/YearSplit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AccumulatedAnnualDemand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AccumulatedAnnualDemand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualEmissionLimit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualEmissionLimit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualExogenousEmission.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AnnualExogenousEmission.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AvailabilityFactor.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/AvailabilityFactor.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityFactor.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityFactor.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityToActivityUnit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapacityToActivityUnit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCostStorage.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/CapitalCostStorage.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaySplit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaySplit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaysInDayType.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/DaysInDayType.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionsPenalty.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/EmissionsPenalty.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FixedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/FixedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/InputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/InputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MinStorageCharge.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/MinStorageCharge.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLife.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OperationalLife.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OutputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/OutputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REMinProductionTarget.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/REMinProductionTarget.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagFuel.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagFuel.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/RETagTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMargin.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMargin.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagFuel.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagFuel.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ReserveMarginTagTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/ResidualCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedAnnualDemand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedAnnualDemand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedDemandProfile.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/SpecifiedDemandProfile.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TECHNOLOGY.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TECHNOLOGY.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacityInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMaxCapacityInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacityInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalAnnualMinCapacityInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityLowerLimit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityLowerLimit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityUpperLimit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/TotalTechnologyAnnualActivityUpperLimit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/VariableCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/VariableCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YearSplit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-complete/YearSplit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityFactor.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityFactor.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityToActivityUnit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapacityToActivityUnit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/CapitalCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaysInDayType.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/DaysInDayType.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionsPenalty.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/EmissionsPenalty.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FixedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/FixedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/InputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/InputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OutputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/OutputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/ResidualCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedAnnualDemand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedAnnualDemand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedDemandProfile.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/SpecifiedDemandProfile.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TECHNOLOGY.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TECHNOLOGY.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacityInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/TotalAnnualMaxCapacityInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/VariableCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/VariableCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YearSplit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-1/YearSplit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityFactor.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityFactor.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityToActivityUnit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapacityToActivityUnit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/CapitalCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaysInDayType.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/DaysInDayType.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionsPenalty.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/EmissionsPenalty.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FixedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/FixedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/InputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/InputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OutputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/OutputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/ResidualCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedAnnualDemand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedAnnualDemand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedDemandProfile.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/SpecifiedDemandProfile.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TECHNOLOGY.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TECHNOLOGY.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacityInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/TotalAnnualMaxCapacityInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/VariableCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/VariableCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YearSplit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-2/YearSplit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityFactor.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityFactor.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityToActivityUnit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapacityToActivityUnit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/CapitalCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaysInDayType.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/DaysInDayType.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionsPenalty.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/EmissionsPenalty.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FixedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/FixedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/InputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/InputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OutputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/OutputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/ResidualCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedAnnualDemand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedAnnualDemand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedDemandProfile.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/SpecifiedDemandProfile.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TECHNOLOGY.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TECHNOLOGY.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacityInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/TotalAnnualMaxCapacityInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/VariableCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/VariableCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YearSplit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-full-electricity-edited-3/YearSplit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/CapitalCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/FixedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/FixedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/InputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/InputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/OutputActivityRatio.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/OutputActivityRatio.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedAnnualDemand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedAnnualDemand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedDemandProfile.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/SpecifiedDemandProfile.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/input_csv/otoole-simple-hydro/YearSplit.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/input_csv/otoole-simple-hydro/YearSplit.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AccumulatedNewCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AccumulatedNewCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualEmissions.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualEmissions.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualFixedOperatingCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualFixedOperatingCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmission.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmission.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmissionByMode.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualTechnologyEmissionByMode.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualVariableOperatingCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/AnnualVariableOperatingCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/CapitalInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/CapitalInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/Demand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/Demand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedSalvageValue.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedSalvageValue.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedTechnologyEmissionsPenalty.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/DiscountedTechnologyEmissionsPenalty.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/NewCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/NewCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnologyAnnual.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/ProductionByTechnologyAnnual.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfActivity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfActivity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnologyByMode.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfProductionByTechnologyByMode.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnologyByMode.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/RateOfUseByTechnologyByMode.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/SalvageValue.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/SalvageValue.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalAnnualTechnologyActivityByMode.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalAnnualTechnologyActivityByMode.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalCapacityAnnual.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalCapacityAnnual.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalDiscountedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalDiscountedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyAnnualActivity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/TotalTechnologyAnnualActivity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-full-electricity/UseByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-full-electricity/UseByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AccumulatedNewCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AccumulatedNewCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualFixedOperatingCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/AnnualFixedOperatingCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/CapitalInvestment.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/CapitalInvestment.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/Demand.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/Demand.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedSalvageValue.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/DiscountedSalvageValue.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/NewCapacity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/NewCapacity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnologyAnnual.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/ProductionByTechnologyAnnual.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfActivity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfActivity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnologyByMode.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfProductionByTechnologyByMode.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnologyByMode.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/RateOfUseByTechnologyByMode.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/SalvageValue.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/SalvageValue.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalAnnualTechnologyActivityByMode.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalAnnualTechnologyActivityByMode.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalCapacityAnnual.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalCapacityAnnual.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalDiscountedCost.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalDiscountedCost.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyAnnualActivity.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/TotalTechnologyAnnualActivity.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/otoole_compat/results_csv/otoole-simple-hydro/UseByTechnology.csv` & `tz_osemosys-0.0.7/examples/otoole_compat/results_csv/otoole-simple-hydro/UseByTechnology.csv`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/quickstart/main.yaml` & `tz_osemosys-0.0.7/examples/quickstart/main.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/examples/utopia/main.yaml` & `tz_osemosys-0.0.7/examples/utopia/main.yaml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/mkdocs.yml` & `tz_osemosys-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/pyproject.toml` & `tz_osemosys-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/fixtures/misc.py` & `tz_osemosys-0.0.7/tests/fixtures/misc.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_commodity.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_commodity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_impact.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_region.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_roundtrip.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_roundtrip.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_runspec.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_runspec.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_storage.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_technology.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_technology.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_compatability/test_otoole_timedef.py` & `tz_osemosys-0.0.7/tests/test_compatability/test_otoole_timedef.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_composition/test_compose_base.py` & `tz_osemosys-0.0.7/tests/test_composition/test_compose_base.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_composition/test_compose_runspec.py` & `tz_osemosys-0.0.7/tests/test_composition/test_compose_runspec.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_base.py` & `tz_osemosys-0.0.7/tests/test_construction/test_base.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_commodity.py` & `tz_osemosys-0.0.7/tests/test_construction/test_commodity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_data.py` & `tz_osemosys-0.0.7/tests/test_construction/test_data.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_impact.py` & `tz_osemosys-0.0.7/tests/test_construction/test_impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_load_from_yaml.py` & `tz_osemosys-0.0.7/tests/test_construction/test_load_from_yaml.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_model.py` & `tz_osemosys-0.0.7/tests/test_construction/test_model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_region.py` & `tz_osemosys-0.0.7/tests/test_construction/test_region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_runspec.py` & `tz_osemosys-0.0.7/tests/test_construction/test_runspec.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_storage.py` & `tz_osemosys-0.0.7/tests/test_construction/test_storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_technology.py` & `tz_osemosys-0.0.7/tests/test_construction/test_technology.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_construction/test_timedefinition.py` & `tz_osemosys-0.0.7/tests/test_construction/test_timedefinition.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_integration/test_linopy_model.py` & `tz_osemosys-0.0.7/tests/test_integration/test_linopy_model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_solve/test_salvage.py` & `tz_osemosys-0.0.7/tests/test_solve/test_salvage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tests/test_solve/test_solve.py` & `tz_osemosys-0.0.7/tests/test_solve/test_solve.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/__init__.py` & `tz_osemosys-0.0.7/tz/osemosys/__init__.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/defaults.py` & `tz_osemosys-0.0.7/tz/osemosys/defaults.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/io/load_model.py` & `tz_osemosys-0.0.7/tz/osemosys/io/load_model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/io/simpleeval.py` & `tz_osemosys-0.0.7/tz/osemosys/io/simpleeval.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/__init__.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import xarray as xr
 from linopy import LinearExpression, Model
 
 from .annual_activity import add_annual_activity_constraints
 from .capacity_adequacy_a import add_capacity_adequacy_a_constraints
 from .capacity_adequacy_b import add_capacity_adequacy_b_constraints
+from .capacity_growth_rate import add_capacity_growthrate_constraints
 from .emissions import add_emissions_constraints
 from .energy_balance_a import add_energy_balance_a_constraints
 from .energy_balance_b import add_energy_balance_b_constraints
 from .new_capacity import add_new_capacity_constraints
 from .re_targets import add_re_targets_constraints
 from .reserve_margin import add_reserve_margin_constraints
 from .storage import add_storage_constraints
@@ -41,9 +42,10 @@
     m = add_annual_activity_constraints(ds, m, lex)
     m = add_new_capacity_constraints(ds, m, lex)
     m = add_re_targets_constraints(ds, m, lex)
     m = add_reserve_margin_constraints(ds, m, lex)
     m = add_storage_constraints(ds, m, lex)
     m = add_total_activity_constraints(ds, m, lex)
     m = add_total_capacity_constraints(ds, m, lex)
+    m = add_capacity_growthrate_constraints(ds, m, lex)
 
     return m
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/_accounting_technology.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/_accounting_technology.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/_capital_costs.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/_capital_costs.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/_operating_costs.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/_operating_costs.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/_salvage_value.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/_salvage_value.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/_total_discounted_costs.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/_total_discounted_costs.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/annual_activity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/annual_activity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/capacity_adequacy_a.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/capacity_adequacy_a.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/capacity_adequacy_b.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/capacity_adequacy_b.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/emissions.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/emissions.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/energy_balance_a.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/energy_balance_a.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/energy_balance_b.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/energy_balance_b.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/new_capacity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/new_capacity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/re_targets.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/re_targets.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/reserve_margin.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/reserve_margin.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/storage.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/total_activity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/total_activity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/constraints/total_capacity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/constraints/total_capacity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/__init__.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/activity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/activity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/capacity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/capacity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/discounting.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/discounting.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/emissions.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/emissions.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/financials.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/financials.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/production.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/production.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/reserve_margin.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/reserve_margin.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/linear_expressions/storage.py` & `tz_osemosys-0.0.7/tz/osemosys/model/linear_expressions/storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/model.py` & `tz_osemosys-0.0.7/tz/osemosys/model/model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/objective.py` & `tz_osemosys-0.0.7/tz/osemosys/model/objective.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/solution.py` & `tz_osemosys-0.0.7/tz/osemosys/model/solution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from typing import Dict
 
 import xarray as xr
 from linopy import LinearExpression, Model
 
 SOLUTION_KEYS = [
+    "AnnualTechnologyEmission",
     "AnnualFixedOperatingCost",
     "AnnualVariableOperatingCost",
     "CapitalInvestment",
     "CapitalInvestmentStorage",
     "DemandNeedingReserveMargin",
     "DiscountedCapitalInvestment",
     "DiscountedCapitalInvestmentStorage",
     "DiscountedOperatingCost",
     "DiscountedSalvageValue",
     "GrossStorageCapacity",
+    "GrossCapacity",
     "NetCharge",
     "NewCapacity",
     "NewStorageCapacity",
     "NumberOfNewTechnologyUnits",
     "OperatingCost",
     "Production",
+    "ProductionByTechnology",
     "SalvageValue",
     "StorageLevel",
     "TotalAnnualTechnologyActivityByMode",
-    "GrossCapacity",
     "TotalCapacityInReserveMargin",
     "TotalDiscountedCost",
     "TotalDiscountedCostByTechnology",
     "TotalDiscountedStorageCost",
     "TotalTechnologyAnnualActivity",
     "TotalTechnologyModelPeriodActivity",
     "Trade",
@@ -111,15 +113,19 @@
     if "StorageLevel" in lex:
         solution_base = solution_base.merge(
             lex["StorageLevel"].solution.unstack("YRTS").rename("StorageLevel")
         )
 
     if solution_vars is None:
         return xr.Dataset(
-            {k: solution_base[k] for k in sorted(list(solution_base.keys())) if k in SOLUTION_KEYS}
+            {
+                k: solution_base[k]
+                for k in sorted(list(solution_base.keys()))
+                if (k in SOLUTION_KEYS) and (k in solution_base.keys())
+            }
         )
     elif solution_vars == "all":
         return xr.Dataset({k: solution_base[k] for k in sorted(list(solution_base.keys()))})
     else:
         # ensure TotalDiscountedCost is always included
         if "TotalDiscountedCost" not in solution_vars:
             solution_vars.append("TotalDiscountedCost")
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/variables/__init__.py` & `tz_osemosys-0.0.7/tz/osemosys/model/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/variables/activity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/variables/activity.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/variables/capacity.py` & `tz_osemosys-0.0.7/tz/osemosys/model/variables/capacity.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,8 +23,21 @@
     # masks
     mask = ds["CapacityOfOneTechnologyUnit"].notnull()
 
     m.add_variables(
         lower=0, upper=inf, coords=RTeY, name="NumberOfNewTechnologyUnits", integer=True, mask=mask
     )
     m.add_variables(lower=0, upper=inf, coords=RTeY, name="NewCapacity", integer=False)
+
+    if (
+        ds["CapacityAdditionalMaxFloor"].notnull().any()
+        and ds["CapacityAdditionalMaxGrowthRate"].notnull().any()
+    ):
+        m.add_variables(
+            lower=0,
+            upper=1,
+            coords=RTeY,
+            name="OR_GrowthRateFloor",
+            integer=True,
+        )
+
     return m
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/model/variables/storage.py` & `tz_osemosys-0.0.7/tz/osemosys/model/variables/storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/base.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/base.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/commodity.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/commodity.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     `demand_profile` `({region:{year:{timeslice:float}})` - OSeMOSYS SpecifiedDemandProfile.
     Specified for a demand which varies by
     timeslice. If `demand_annual` is given for a commodity but `demand_profile` is not, the demand
     is treated as having an accumulated demand, which must be met for each year within any
     combination of timeslices. Optional, defaults to `None`.
 
-    `is_renewable` `({region:{year:bool}})` - OSeMOSYS RETagFuel.
+    `include_in_joint_renewable_target` `({region:{year:bool}})` - OSeMOSYS RETagFuel.
     Boolean tag to mark commodities which are considered
     as renewable for applying renewable generation targets. Optional, defaults to `None`.
 
 
 
     ## Examples
 
@@ -75,15 +75,15 @@
 
     `check_demand_exists_if_profile` - This enforces that if `demand_profile` is defined for a
     region and year, `demand_annual` must also be defined.
     """
 
     demand_annual: OSeMOSYSData.RY | None = Field(None)
     demand_profile: OSeMOSYSData.RYS.SumOne | None = Field(None)
-    is_renewable: OSeMOSYSData.RY.Bool | None = Field(None)
+    include_in_joint_renewable_target: OSeMOSYSData.RY.Bool | None = Field(None)
 
     # include this technology in joint reserve margin and renewables targets
     include_in_joint_reserve_margin: OSeMOSYSData.RY.Bool | None = Field(None)
     include_in_joint_renewable_target: OSeMOSYSData.RY.Bool | None = Field(None)
 
     @model_validator(mode="before")
     @classmethod
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/base.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/base.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/commodity.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/commodity.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             "columns": ["REGION", "FUEL", "TIMESLICE", "YEAR", "VALUE"],
         },
         "AccumulatedAnnualDemand": {
             "attribute": "accumulated_demand",
             "columns": ["REGION", "FUEL", "YEAR", "VALUE"],
         },
         "RETagFuel": {
-            "attribute": "is_renewable",
+            "attribute": "include_in_joint_renewable_target",
             "columns": ["REGION", "FUEL", "YEAR", "VALUE"],
         },
     }
 
     @classmethod
     def from_otoole_csv(cls, root_dir):
         # ###########
@@ -126,15 +126,15 @@
                         data_columns=["REGION", "YEAR", "TIMESLICE"],
                         target_column="VALUE",
                     )
                 )
                 if commodity in dfs["SpecifiedDemandProfile"]["FUEL"].values
                 else None
             )
-            is_renewable = (
+            include_in_joint_renewable_target = (
                 OSeMOSYSData.RY.Bool(
                     group_to_json(
                         g=dfs["RETagFuel"].loc[dfs["RETagFuel"]["FUEL"] == commodity],
                         root_column="FUEL",
                         data_columns=["REGION", "YEAR"],
                         target_column="VALUE",
                     )
@@ -155,15 +155,15 @@
 
             commodity_instances.append(
                 cls(
                     id=commodity,
                     otoole_cfg=otoole_cfg,
                     demand_annual=demand,
                     demand_profile=demand_profile,
-                    is_renewable=is_renewable,
+                    include_in_joint_renewable_target=include_in_joint_renewable_target,
                 )
             )
 
         return commodity_instances
 
     @classmethod
     def to_dataframes(cls, commodities: List["Commodity"]):
@@ -173,15 +173,15 @@
         dfs["FUEL"] = pd.DataFrame({"VALUE": [commodity.id for commodity in commodities]})
 
         # Parameters
         # collect demand dataframes
         accumulated_demand_dfs = []
         annual_demand_dfs = []
         demand_profile_dfs = []
-        is_renewable_dfs = []
+        include_in_joint_renewable_target_dfs = []
 
         for commodity in commodities:
             if commodity.demand_annual is not None:
                 df = pd.json_normalize(commodity.demand_annual.data).T.rename(columns={0: "VALUE"})
                 df["FUEL"] = commodity.id
                 df[["REGION", "YEAR"]] = pd.DataFrame(
                     df.index.str.split(".").to_list(), index=df.index
@@ -195,33 +195,36 @@
 
                             # ... and add profile df to demand_profile_dfs
                             df_profile = pd.json_normalize(commodity.demand_profile.data).T.rename(
                                 columns={0: "VALUE"}
                             )
                             df_profile["FUEL"] = commodity.id
                             df_profile[["REGION", "YEAR", "TIMESLICE"]] = pd.DataFrame(
-                                df_profile.index.str.split(".").to_list(), index=df_profile.index
+                                df_profile.index.str.split(".").to_list(),
+                                index=df_profile.index,
                             )
                             demand_profile_dfs.append(
                                 df_profile.loc[df_profile["REGION"] == region]
                             )
                         else:
                             accumulated_demand_dfs.append(df.loc[df["REGION"] == region])
                 # If no demand_profile, put all data in accumulated demand
                 else:
                     accumulated_demand_dfs.append(df)
 
-            if commodity.is_renewable is not None:
-                df = pd.json_normalize(commodity.is_renewable.data).T.rename(columns={0: "VALUE"})
+            if commodity.include_in_joint_renewable_target is not None:
+                df = pd.json_normalize(commodity.include_in_joint_renewable_target.data).T.rename(
+                    columns={0: "VALUE"}
+                )
                 df["FUEL"] = commodity.id
                 df[["REGION", "YEAR"]] = pd.DataFrame(
                     df.index.str.split(".").to_list(), index=df.index
                 )
                 df["VALUE"] = df["VALUE"].map({True: 1, False: 0})
-                is_renewable_dfs.append(df)
+                include_in_joint_renewable_target_dfs.append(df)
 
         dfs["SpecifiedAnnualDemand"] = (
             pd.concat(annual_demand_dfs)
             if annual_demand_dfs
             else pd.DataFrame(columns=cls.otoole_stems["SpecifiedAnnualDemand"]["columns"])
         )
         dfs["AccumulatedAnnualDemand"] = (
@@ -231,16 +234,16 @@
         )
         dfs["SpecifiedDemandProfile"] = (
             pd.concat(demand_profile_dfs)
             if demand_profile_dfs
             else pd.DataFrame(columns=cls.otoole_stems["SpecifiedDemandProfile"]["columns"])
         )
         dfs["RETagFuel"] = (
-            pd.concat(is_renewable_dfs)
-            if is_renewable_dfs
+            pd.concat(include_in_joint_renewable_target_dfs)
+            if include_in_joint_renewable_target_dfs
             else pd.DataFrame(columns=cls.otoole_stems["RETagFuel"]["columns"])
         )
 
         return dfs
 
     @classmethod
     def to_otoole_csv(cls, commodities: List["Commodity"], output_directory: str):
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/impact.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/model.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/model.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/region.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/storage.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/technology.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/technology.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,26 @@
 class OtooleTechnology(BaseModel):
     """
     Class to contain methods for converting Technology data to and from otoole style CSVs
     """
 
     otoole_cfg: OtooleCfg | None = Field(None)
     otoole_stems: ClassVar[dict[str : dict[str : Union[str, list[str]]]]] = {
+        "CapacityAdditionalMaxGrowthRate": {
+            "attribute": "capacity_additional_max_growth_rate",
+            "columns": ["REGION", "TECHNOLOGY", "VALUE"],
+        },
+        "CapacityAdditionalMinGrowthRate": {
+            "attribute": "capacity_additional_min_growth_rate",
+            "columns": ["REGION", "TECHNOLOGY", "VALUE"],
+        },
+        "CapacityAdditionalMaxFloor": {
+            "attribute": "capacity_additional_max_floor",
+            "columns": ["REGION", "TECHNOLOGY", "VALUE"],
+        },
         "CapacityToActivityUnit": {
             "attribute": "capacity_activity_unit_ratio",
             "columns": ["REGION", "TECHNOLOGY", "VALUE"],
         },
         "CapacityOfOneTechnologyUnit": {
             "attribute": "capacity_one_tech_unit",
             "columns": ["REGION", "TECHNOLOGY", "YEAR", "VALUE"],
@@ -121,22 +133,34 @@
                 "FUEL",
                 "YEAR",
                 "VALUE",
             ],
         },
         "TechnologyToStorage": {
             "attribute": "to_storage",
-            "columns": ["MODE_OF_OPERATION", "REGION", "TECHNOLOGY", "STORAGE", "VALUE"],
+            "columns": [
+                "MODE_OF_OPERATION",
+                "REGION",
+                "TECHNOLOGY",
+                "STORAGE",
+                "VALUE",
+            ],
         },
         "TechnologyFromStorage": {
             "attribute": "from_storage",
-            "columns": ["MODE_OF_OPERATION", "REGION", "TECHNOLOGY", "STORAGE", "VALUE"],
+            "columns": [
+                "MODE_OF_OPERATION",
+                "REGION",
+                "TECHNOLOGY",
+                "STORAGE",
+                "VALUE",
+            ],
         },
         "RETagTechnology": {
-            "attribute": "is_renewable",
+            "attribute": "include_in_joint_renewable_target",
             "columns": ["REGION", "TECHNOLOGY", "YEAR", "VALUE"],
         },
     }
     operating_mode_stem_translation: ClassVar[dict[str, str]] = {
         "VariableCost": ("opex_variable", OSeMOSYSData.RY),
         "EmissionActivityRatio": ("emission_activity_ratio", OSeMOSYSData.RIY),
         "InputActivityRatio": ("input_activity_ratio", OSeMOSYSData.RCY),
@@ -324,15 +348,15 @@
                         OSeMOSYSData.R(
                             data=data_json_format["TotalTechnologyModelPeriodActivityLowerLimit"]
                         )
                         if data_json_format["TotalTechnologyModelPeriodActivityLowerLimit"]
                         is not None
                         else None
                     ),
-                    is_renewable=(
+                    include_in_joint_renewable_target=(
                         OSeMOSYSData.RY.Bool(data=data_json_format["RETagTechnology"])
                         if data_json_format["RETagTechnology"] is not None
                         else None
                     ),
                 )
             )
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/compat/time_definition.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/compat/time_definition.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/impact.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/impact.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/model.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,17 @@
     `reserve_margin` `({region:{year:float}})` - OSeMOSYS ReserveMargin.
     Minimum level of the reserve margin required to be provided for all the tagged commodities, by
     the tagged technologies. If no reserve margin is required, the parameter will have value 1; if,
     for instance, 20% reserve margin is required, the parameter will have value 1.2.
     Optional parameter, defaults to 1.
 
     `renewable_production_target` `({region:{year:float}})` - OSeMOSYS REMinProductionTarget.
-    Minimum ratio of all renewable commodities tagged in the is_renewable parameter, to be
-    produced by the technologies tagged with the is_renewable parameter.
+    Minimum ratio of all renewable commodities tagged in the
+    include_in_joint_renewable_target parameter, to be
+    produced by the technologies tagged with the include_in_joint_renewable_target parameter.
     Optional parameter, defaults to `None`.
 
     ## Examples
 
     ### From dicts
 
     A simple example of how a Runspec object might be created directly from provided data is below:
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/region.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/region.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/storage.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/storage.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/technology.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/technology.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     Optional, defaults to 1.
 
     `capacity_one_tech_unit` `({region:{year:float}})` - OSeMOSYS CapacityOfOneTechnologyUnit.
     Capacity of one new unit of a technology. In case the user sets this parameter, the related
     technology will be installed only in batches of the specified capacity and the problem will
     turn into a Mixed Integer Linear Problem. Optional, defaults to `None`.
 
-    `is_renewable` `({region:{year:bool}})` - OSeMOSYS RETagTechnology.
+    `include_in_joint_renewable_target` `({region:{year:bool}})` - OSeMOSYS RETagTechnology.
     Boolean tagging the renewable technologies that must contribute to reaching the indicated
     minimum renewable production target. It has value True for thetechnologies contributing,
     False otherwise. Optional, defaults to `None`.
 
     `capacity_gross_max` `({region:{year:float}})` - OSeMOSYS TotalAnnualMaxCapacity.
     Total maximum existing (residual plus cumulatively installed) capacity allowed for a technology
     in a specified year. Optional, defaults to `None`.
@@ -262,29 +262,32 @@
         OSeMOSYSData.RY(defaults.technology_availability_factor)
     )
     capacity_factor: OSeMOSYSData.RYS = Field(OSeMOSYSData.RYS(defaults.technology_capacity_factor))
 
     # NON-REQUIRED PARAMETERS
 
     capacity_one_tech_unit: OSeMOSYSData.RY | None = Field(None)
-    is_renewable: OSeMOSYSData.RY.Bool | None = Field(None)
+    include_in_joint_renewable_target: OSeMOSYSData.RY.Bool | None = Field(None)
 
     # NON-REQUIRED CONSTRAINTS
     # -----
-    # capacity
+    # gross capacity max/min in each year
     capacity_gross_max: OSeMOSYSData.RY | None = Field(None)
     capacity_gross_min: OSeMOSYSData.RY | None = Field(None)
+
+    # additional capacity upper bounds
     capacity_additional_max: OSeMOSYSData.RY | None = Field(None)
-    capacity_additional_min: OSeMOSYSData.RY | None = Field(None)
+    capacity_additional_max_growth_rate: OSeMOSYSData.R | None = Field(None)
+    # upper bound floor: if used with growth_rate,
+    # limits capacity growth to the floor or growth-rate, whichever is greater
+    capacity_additional_max_floor: OSeMOSYSData.R | None = Field(None)
 
-    # growth rate # TO BE IMPLEMENTED
-    # capacity_additional_max_growth_rate: OSeMOSYSData | None  = Field(None)
-    # capacity_additional_max_ceil: OSeMOSYSData | None = Field(None)
-    # capacity_additional_max_floor: RegionYearData | None = Field(None)
-    # capacity_additional_min_growth_rate: RegionYearData | None  = Field(None)
+    # additional capacity lower bounds (MUST build)
+    capacity_additional_min: OSeMOSYSData.RY | None = Field(None)
+    capacity_additional_min_growth_rate: OSeMOSYSData.R | None = Field(None)
 
     # activity
     activity_annual_max: OSeMOSYSData.RY | None = Field(None)
     activity_annual_min: OSeMOSYSData.RY | None = Field(None)
     activity_total_max: OSeMOSYSData.R | None = Field(None)
     activity_total_min: OSeMOSYSData.R | None = Field(None)
```

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/time_definition.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/time_definition.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/validation/impact_validation.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/validation/impact_validation.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/validation/model_composition.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/validation/model_composition.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/validation/model_presolve.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/validation/model_presolve.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/validation/region_validation.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/validation/region_validation.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/validation/technology_validation.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/validation/technology_validation.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/validation/timedefinition_validation.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/validation/timedefinition_validation.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/schemas/validation/validation_utils.py` & `tz_osemosys-0.0.7/tz/osemosys/schemas/validation/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/utils/__init__.py` & `tz_osemosys-0.0.7/tz/osemosys/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/utils/cfg_parser.py` & `tz_osemosys-0.0.7/tz/osemosys/utils/cfg_parser.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz/osemosys/utils/utils.py` & `tz_osemosys-0.0.7/tz/osemosys/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tz_osemosys-0.0.5/tz_osemosys.egg-info/PKG-INFO` & `tz_osemosys-0.0.7/tz_osemosys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tz-osemosys
-Version: 0.0.5
+Version: 0.0.7
 Summary: An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero
 Author-email: Lucas Kruitwagen <lucas.kruitwagen@gmail.com>, Ed Gill <edwardxtg@gmail.com>, Abhishek Shivakumar <abhishek0208@gmail.com>
 Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org
 Project-URL: Source, https://github.com/transitionzero/tz-osemosys
 Keywords: energy,milp,climate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.5 Summary: An OSeMOSYS
+Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.7 Summary: An OSeMOSYS
 implementation for the Future Energy Outlook by TransitionZero Author-email:
 Lucas Kruitwagen
 gmail.com>, Ed Gill
 gmail.com>, Abhishek Shivakumar
 gmail.com> Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org Project-URL: Source, https://
```

### Comparing `tz_osemosys-0.0.5/tz_osemosys.egg-info/SOURCES.txt` & `tz_osemosys-0.0.7/tz_osemosys.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -479,14 +479,127 @@
 examples/quickstart/main.yaml
 examples/utopia/main.yaml
 tests/__init__.py
 tests/conftest.py
 tests/fixtures/__init__.py
 tests/fixtures/misc.py
 tests/fixtures/paths.py
+tests/otoole_compare/otoole-full-electricity/CapacityFactor.csv
+tests/otoole_compare/otoole-full-electricity/CapacityToActivityUnit.csv
+tests/otoole_compare/otoole-full-electricity/CapitalCost.csv
+tests/otoole_compare/otoole-full-electricity/Conversionld.csv
+tests/otoole_compare/otoole-full-electricity/Conversionls.csv
+tests/otoole_compare/otoole-full-electricity/DAYTYPE.csv
+tests/otoole_compare/otoole-full-electricity/DaysInDayType.csv
+tests/otoole_compare/otoole-full-electricity/EMISSION.csv
+tests/otoole_compare/otoole-full-electricity/EmissionActivityRatio.csv
+tests/otoole_compare/otoole-full-electricity/EmissionsPenalty.csv
+tests/otoole_compare/otoole-full-electricity/FUEL.csv
+tests/otoole_compare/otoole-full-electricity/FixedCost.csv
+tests/otoole_compare/otoole-full-electricity/InputActivityRatio.csv
+tests/otoole_compare/otoole-full-electricity/MODE_OF_OPERATION.csv
+tests/otoole_compare/otoole-full-electricity/OperationalLife.csv
+tests/otoole_compare/otoole-full-electricity/OutputActivityRatio.csv
+tests/otoole_compare/otoole-full-electricity/REGION.csv
+tests/otoole_compare/otoole-full-electricity/ResidualCapacity.csv
+tests/otoole_compare/otoole-full-electricity/SEASON.csv
+tests/otoole_compare/otoole-full-electricity/STORAGE.csv
+tests/otoole_compare/otoole-full-electricity/SpecifiedAnnualDemand.csv
+tests/otoole_compare/otoole-full-electricity/SpecifiedDemandProfile.csv
+tests/otoole_compare/otoole-full-electricity/TECHNOLOGY.csv
+tests/otoole_compare/otoole-full-electricity/TIMESLICE.csv
+tests/otoole_compare/otoole-full-electricity/TotalAnnualMaxCapacity.csv
+tests/otoole_compare/otoole-full-electricity/TotalAnnualMaxCapacityInvestment.csv
+tests/otoole_compare/otoole-full-electricity/VariableCost.csv
+tests/otoole_compare/otoole-full-electricity/YEAR.csv
+tests/otoole_compare/otoole-full-electricity/YearSplit.csv
+tests/otoole_compare/otoole-full-electricity/_REGION.csv
+tests/otoole_compare/otoole-full-electricity-complete/AccumulatedAnnualDemand.csv
+tests/otoole_compare/otoole-full-electricity-complete/AnnualEmissionLimit.csv
+tests/otoole_compare/otoole-full-electricity-complete/AnnualExogenousEmission.csv
+tests/otoole_compare/otoole-full-electricity-complete/AvailabilityFactor.csv
+tests/otoole_compare/otoole-full-electricity-complete/CapacityFactor.csv
+tests/otoole_compare/otoole-full-electricity-complete/CapacityToActivityUnit.csv
+tests/otoole_compare/otoole-full-electricity-complete/CapitalCost.csv
+tests/otoole_compare/otoole-full-electricity-complete/CapitalCostStorage.csv
+tests/otoole_compare/otoole-full-electricity-complete/Conversionld.csv
+tests/otoole_compare/otoole-full-electricity-complete/Conversionlh.csv
+tests/otoole_compare/otoole-full-electricity-complete/Conversionls.csv
+tests/otoole_compare/otoole-full-electricity-complete/DAILYTIMEBRACKET.csv
+tests/otoole_compare/otoole-full-electricity-complete/DAYTYPE.csv
+tests/otoole_compare/otoole-full-electricity-complete/DaySplit.csv
+tests/otoole_compare/otoole-full-electricity-complete/DaysInDayType.csv
+tests/otoole_compare/otoole-full-electricity-complete/DepreciationMethod.csv
+tests/otoole_compare/otoole-full-electricity-complete/DiscountRate.csv
+tests/otoole_compare/otoole-full-electricity-complete/DiscountRateIdv.csv
+tests/otoole_compare/otoole-full-electricity-complete/DiscountRateStorage.csv
+tests/otoole_compare/otoole-full-electricity-complete/EMISSION.csv
+tests/otoole_compare/otoole-full-electricity-complete/EmissionActivityRatio.csv
+tests/otoole_compare/otoole-full-electricity-complete/EmissionsPenalty.csv
+tests/otoole_compare/otoole-full-electricity-complete/FUEL.csv
+tests/otoole_compare/otoole-full-electricity-complete/FixedCost.csv
+tests/otoole_compare/otoole-full-electricity-complete/InputActivityRatio.csv
+tests/otoole_compare/otoole-full-electricity-complete/MODE_OF_OPERATION.csv
+tests/otoole_compare/otoole-full-electricity-complete/MinStorageCharge.csv
+tests/otoole_compare/otoole-full-electricity-complete/ModelPeriodEmissionLimit.csv
+tests/otoole_compare/otoole-full-electricity-complete/ModelPeriodExogenousEmission.csv
+tests/otoole_compare/otoole-full-electricity-complete/OperationalLife.csv
+tests/otoole_compare/otoole-full-electricity-complete/OperationalLifeStorage.csv
+tests/otoole_compare/otoole-full-electricity-complete/OutputActivityRatio.csv
+tests/otoole_compare/otoole-full-electricity-complete/REGION.csv
+tests/otoole_compare/otoole-full-electricity-complete/REMinProductionTarget.csv
+tests/otoole_compare/otoole-full-electricity-complete/RETagFuel.csv
+tests/otoole_compare/otoole-full-electricity-complete/RETagTechnology.csv
+tests/otoole_compare/otoole-full-electricity-complete/ReserveMargin.csv
+tests/otoole_compare/otoole-full-electricity-complete/ReserveMarginTagFuel.csv
+tests/otoole_compare/otoole-full-electricity-complete/ReserveMarginTagTechnology.csv
+tests/otoole_compare/otoole-full-electricity-complete/ResidualCapacity.csv
+tests/otoole_compare/otoole-full-electricity-complete/ResidualStorageCapacity.csv
+tests/otoole_compare/otoole-full-electricity-complete/SEASON.csv
+tests/otoole_compare/otoole-full-electricity-complete/STORAGE.csv
+tests/otoole_compare/otoole-full-electricity-complete/SpecifiedAnnualDemand.csv
+tests/otoole_compare/otoole-full-electricity-complete/SpecifiedDemandProfile.csv
+tests/otoole_compare/otoole-full-electricity-complete/StorageLevelStart.csv
+tests/otoole_compare/otoole-full-electricity-complete/StorageMaxChargeRate.csv
+tests/otoole_compare/otoole-full-electricity-complete/StorageMaxDischargeRate.csv
+tests/otoole_compare/otoole-full-electricity-complete/TECHNOLOGY.csv
+tests/otoole_compare/otoole-full-electricity-complete/TIMESLICE.csv
+tests/otoole_compare/otoole-full-electricity-complete/TechnologyFromStorage.csv
+tests/otoole_compare/otoole-full-electricity-complete/TechnologyToStorage.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMaxCapacity.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMaxCapacityInvestment.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMinCapacity.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalAnnualMinCapacityInvestment.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyAnnualActivityLowerLimit.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyAnnualActivityUpperLimit.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityLowerLimit.csv
+tests/otoole_compare/otoole-full-electricity-complete/TotalTechnologyModelPeriodActivityUpperLimit.csv
+tests/otoole_compare/otoole-full-electricity-complete/TradeRoute.csv
+tests/otoole_compare/otoole-full-electricity-complete/VariableCost.csv
+tests/otoole_compare/otoole-full-electricity-complete/YEAR.csv
+tests/otoole_compare/otoole-full-electricity-complete/YearSplit.csv
+tests/otoole_compare/otoole-full-electricity-complete/_REGION.csv
+tests/otoole_compare/otoole-simple-hydro/CapacityToActivityUnit.csv
+tests/otoole_compare/otoole-simple-hydro/CapitalCost.csv
+tests/otoole_compare/otoole-simple-hydro/EMISSION.csv
+tests/otoole_compare/otoole-simple-hydro/FUEL.csv
+tests/otoole_compare/otoole-simple-hydro/FixedCost.csv
+tests/otoole_compare/otoole-simple-hydro/InputActivityRatio.csv
+tests/otoole_compare/otoole-simple-hydro/MODE_OF_OPERATION.csv
+tests/otoole_compare/otoole-simple-hydro/OperationalLife.csv
+tests/otoole_compare/otoole-simple-hydro/OutputActivityRatio.csv
+tests/otoole_compare/otoole-simple-hydro/REGION.csv
+tests/otoole_compare/otoole-simple-hydro/STORAGE.csv
+tests/otoole_compare/otoole-simple-hydro/SpecifiedAnnualDemand.csv
+tests/otoole_compare/otoole-simple-hydro/SpecifiedDemandProfile.csv
+tests/otoole_compare/otoole-simple-hydro/TECHNOLOGY.csv
+tests/otoole_compare/otoole-simple-hydro/TIMESLICE.csv
+tests/otoole_compare/otoole-simple-hydro/YEAR.csv
+tests/otoole_compare/otoole-simple-hydro/YearSplit.csv
+tests/otoole_compare/otoole-simple-hydro/_REGION.csv
 tests/test_compatability/test_otoole_commodity.py
 tests/test_compatability/test_otoole_impact.py
 tests/test_compatability/test_otoole_region.py
 tests/test_compatability/test_otoole_roundtrip.py
 tests/test_compatability/test_otoole_runspec.py
 tests/test_compatability/test_otoole_storage.py
 tests/test_compatability/test_otoole_technology.py
@@ -501,14 +614,15 @@
 tests/test_construction/test_model.py
 tests/test_construction/test_region.py
 tests/test_construction/test_runspec.py
 tests/test_construction/test_storage.py
 tests/test_construction/test_technology.py
 tests/test_construction/test_timedefinition.py
 tests/test_integration/test_linopy_model.py
+tests/test_solve/test_growth_rates.py
 tests/test_solve/test_salvage.py
 tests/test_solve/test_solve.py
 tests/test_solve/test_to_xr_ds.py
 tz/osemosys/__init__.py
 tz/osemosys/defaults.py
 tz/osemosys/exceptions.py
 tz/osemosys/logger.py
@@ -524,14 +638,15 @@
 tz/osemosys/model/constraints/_capital_costs.py
 tz/osemosys/model/constraints/_operating_costs.py
 tz/osemosys/model/constraints/_salvage_value.py
 tz/osemosys/model/constraints/_total_discounted_costs.py
 tz/osemosys/model/constraints/annual_activity.py
 tz/osemosys/model/constraints/capacity_adequacy_a.py
 tz/osemosys/model/constraints/capacity_adequacy_b.py
+tz/osemosys/model/constraints/capacity_growth_rate.py
 tz/osemosys/model/constraints/emissions.py
 tz/osemosys/model/constraints/energy_balance_a.py
 tz/osemosys/model/constraints/energy_balance_b.py
 tz/osemosys/model/constraints/new_capacity.py
 tz/osemosys/model/constraints/re_targets.py
 tz/osemosys/model/constraints/reserve_margin.py
 tz/osemosys/model/constraints/storage.py
```

