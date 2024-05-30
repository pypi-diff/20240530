# Comparing `tmp/oasislmf-2.3.2.tar.gz` & `tmp/oasislmf-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasislmf-2.3.2.tar", last modified: Wed Mar 27 15:41:13 2024, max compression
+gzip compressed data, was "oasislmf-2.3.4.tar", last modified: Mon Apr 29 11:43:49 2024, max compression
```

## Comparing `oasislmf-2.3.2.tar` & `oasislmf-2.3.4.tar`

### file list

```diff
@@ -1,186 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.038360 oasislmf-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    85289 2024-03-27 15:41:02.000000 oasislmf-2.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-27 15:41:02.000000 oasislmf-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-27 15:41:02.000000 oasislmf-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-27 15:41:13.038360 oasislmf-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-03-27 15:41:02.000000 oasislmf-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.018360 oasislmf-2.3.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5844 2024-03-27 15:41:02.000000 oasislmf-2.3.2/bin/completer_oasislmf
--rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-03-27 15:41:02.000000 oasislmf-2.3.2/bin/ktools_monitor.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.018360 oasislmf-2.3.2/oasislmf/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.018360 oasislmf-2.3.2/oasislmf/_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/analysis_settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/calc_rules_direct.csv
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/calc_rules_direct_layer.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/calc_rules_step.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/config_compatibility_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)    30010 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/default_acc_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)    23493 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/default_combined_exposure_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/default_fm_agg_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/default_fm_profile_field_values.json
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/default_loc_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/default_step_policies_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/_data/quantile.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/computation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/computation/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/computation/data/dummy_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/data/dummy_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/data/dummy_model/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/computation/generate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33247 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/generate/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/generate/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    56277 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/generate/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/computation/helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/helper/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/computation/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/hooks/post_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/hooks/pre_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.022360 oasislmf-2.3.2/oasislmf/computation/run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21576 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/run/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/run/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/run/generate_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/run/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17347 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/computation/run/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.026360 oasislmf-2.3.2/oasislmf/execution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   103271 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/bin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1271 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/complex_items_to_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/complex_items_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/execution/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.026360 oasislmf-2.3.2/oasislmf/lookup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/lookup/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/lookup/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)    25727 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/lookup/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/lookup/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.026360 oasislmf-2.3.2/oasislmf/platform_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/platform_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27400 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/platform_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/platform_api/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.026360 oasislmf-2.3.2/oasislmf/preparation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/dir_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26073 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/gul_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52210 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/il_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/oed.py
--rw-r--r--   0 runner    (1001) docker     (127)    35747 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/reinsurance_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    38822 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/preparation/summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.030360 oasislmf-2.3.2/oasislmf/pytools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/cdftocsv.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/compare_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/correlationtobin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/correlationtocsv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.030360 oasislmf-2.3.2/oasislmf/pytools/data_layer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/data_layer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.030360 oasislmf-2.3.2/oasislmf/pytools/data_layer/conversions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/data_layer/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/data_layer/conversions/correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/data_layer/conversions/footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/data_layer/footprint_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.030360 oasislmf-2.3.2/oasislmf/pytools/data_layer/oasis_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/data_layer/oasis_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/data_layer/oasis_files/correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/dfcompare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.030360 oasislmf-2.3.2/oasislmf/pytools/fm/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/back_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)    44690 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/compute_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    30859 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/financial_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    33898 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/policy_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    17062 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fm/stream_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/fmpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/footprintconv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.034360 oasislmf-2.3.2/oasislmf/pytools/getmodel/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/getmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/getmodel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/getmodel/footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    40351 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/getmodel/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/getmodel/vulnerability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.034360 oasislmf-2.3.2/oasislmf/pytools/gul/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gul/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gul/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    16315 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gul/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    24497 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gul/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gul/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gul/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.034360 oasislmf-2.3.2/oasislmf/pytools/gulmc/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gulmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gulmc/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gulmc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gulmc/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gulmc/items.py
--rw-r--r--   0 runner    (1001) docker     (127)    77037 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gulmc/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/gulpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/modelpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.034360 oasislmf-2.3.2/oasislmf/pytools/pla/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/pla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/pla/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/pla/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/pla/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/pla/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/plapy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/pytools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.038360 oasislmf-2.3.2/oasislmf/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/calc_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/coverages.py
--rw-r--r--   0 runner    (1001) docker     (127)    38143 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/fm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/peril.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/utils/version_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.038360 oasislmf-2.3.2/oasislmf/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-27 15:41:02.000000 oasislmf-2.3.2/oasislmf/validation/model_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:41:13.018360 oasislmf-2.3.2/oasislmf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-27 15:41:12.000000 oasislmf-2.3.2/oasislmf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-03-27 15:41:13.000000 oasislmf-2.3.2/oasislmf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:41:12.000000 oasislmf-2.3.2/oasislmf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-27 15:41:12.000000 oasislmf-2.3.2/oasislmf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-27 15:41:12.000000 oasislmf-2.3.2/oasislmf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 15:41:12.000000 oasislmf-2.3.2/oasislmf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-27 15:41:02.000000 oasislmf-2.3.2/optional-package.in
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 15:41:02.000000 oasislmf-2.3.2/requirements-package.in
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-27 15:41:13.038360 oasislmf-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    14799 2024-03-27 15:41:02.000000 oasislmf-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.185359 oasislmf-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    86049 2024-04-29 11:43:43.000000 oasislmf-2.3.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-29 11:43:43.000000 oasislmf-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-29 11:43:43.000000 oasislmf-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-29 11:43:49.185359 oasislmf-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-04-29 11:43:43.000000 oasislmf-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.165359 oasislmf-2.3.4/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5844 2024-04-29 11:43:43.000000 oasislmf-2.3.4/bin/completer_oasislmf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-04-29 11:43:43.000000 oasislmf-2.3.4/bin/ktools_monitor.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.165359 oasislmf-2.3.4/oasislmf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/analysis_settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/calc_rules_direct.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/calc_rules_direct_layer.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/calc_rules_step.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/config_compatibility_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30010 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/default_acc_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23493 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/default_combined_exposure_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/default_fm_agg_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/default_fm_profile_field_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/default_loc_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/default_step_policies_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/_data/quantile.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/computation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/computation/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/computation/data/dummy_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/data/dummy_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/data/dummy_model/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/computation/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33247 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/generate/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/generate/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58502 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/generate/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/computation/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/helper/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.169359 oasislmf-2.3.4/oasislmf/computation/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/hooks/post_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/hooks/pre_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.173359 oasislmf-2.3.4/oasislmf/computation/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21576 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/run/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/run/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/run/generate_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/run/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17347 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/computation/run/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.173359 oasislmf-2.3.4/oasislmf/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103926 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26945 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/complex_items_to_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/complex_items_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/execution/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.173359 oasislmf-2.3.4/oasislmf/lookup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/lookup/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/lookup/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25727 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/lookup/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/lookup/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.173359 oasislmf-2.3.4/oasislmf/platform_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/platform_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27400 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/platform_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/platform_api/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.177359 oasislmf-2.3.4/oasislmf/preparation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/dir_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26073 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/gul_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52210 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/il_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/oed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35747 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/reinsurance_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38822 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/preparation/summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.177359 oasislmf-2.3.4/oasislmf/pytools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/cdftocsv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.177359 oasislmf-2.3.4/oasislmf/pytools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/common/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15448 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/common/event_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/compare_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/correlationtobin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/correlationtocsv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.177359 oasislmf-2.3.4/oasislmf/pytools/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/data_layer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.177359 oasislmf-2.3.4/oasislmf/pytools/data_layer/conversions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/data_layer/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/data_layer/conversions/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/data_layer/conversions/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12069 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/data_layer/footprint_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.177359 oasislmf-2.3.4/oasislmf/pytools/data_layer/oasis_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/data_layer/oasis_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/data_layer/oasis_files/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/dfcompare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.181359 oasislmf-2.3.4/oasislmf/pytools/fm/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15426 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/back_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44673 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/compute_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29645 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/financial_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33898 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/policy_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13298 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/fm/stream_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/footprintconv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.181359 oasislmf-2.3.4/oasislmf/pytools/getmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/getmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/getmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13909 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/getmodel/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40364 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/getmodel/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/getmodel/vulnerability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.181359 oasislmf-2.3.4/oasislmf/pytools/gul/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gul/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gul/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gul/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24398 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gul/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gul/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gul/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.181359 oasislmf-2.3.4/oasislmf/pytools/gulmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gulmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gulmc/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gulmc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gulmc/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gulmc/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72381 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gulmc/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/gulpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/modelpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.185359 oasislmf-2.3.4/oasislmf/pytools/pla/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/pla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/pla/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/pla/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/pla/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/pla/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/pla/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.185359 oasislmf-2.3.4/oasislmf/pytools/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/summary/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26466 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/summary/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/pytools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.185359 oasislmf-2.3.4/oasislmf/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/calc_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/coverages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38143 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/fm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/peril.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/utils/version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.185359 oasislmf-2.3.4/oasislmf/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-29 11:43:43.000000 oasislmf-2.3.4/oasislmf/validation/model_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:43:49.165359 oasislmf-2.3.4/oasislmf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-29 11:43:49.000000 oasislmf-2.3.4/oasislmf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-29 11:43:49.000000 oasislmf-2.3.4/oasislmf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:43:49.000000 oasislmf-2.3.4/oasislmf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-29 11:43:49.000000 oasislmf-2.3.4/oasislmf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-29 11:43:49.000000 oasislmf-2.3.4/oasislmf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 11:43:49.000000 oasislmf-2.3.4/oasislmf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 11:43:43.000000 oasislmf-2.3.4/optional-package.in
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-29 11:43:43.000000 oasislmf-2.3.4/requirements-package.in
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-29 11:43:49.185359 oasislmf-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    14862 2024-04-29 11:43:43.000000 oasislmf-2.3.4/setup.py
```

### Comparing `oasislmf-2.3.2/CHANGELOG.rst` & `oasislmf-2.3.4/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 OasisLMF Changelog
 ==================
 
+`2.3.2`_
+ ---------
+* [#1471](https://github.com/OasisLMF/OasisLMF/pull/1472) - number_of_samples = 0 not working in oasislmf
+* [#1473](https://github.com/OasisLMF/OasisLMF/pull/1473) - ajust vuln index after vuln_dict has the updated indexes
+* [#1474](https://github.com/OasisLMF/OasisLMF/pull/1474) - Use billiard package for keys multiprocess if available
+* [#1481](https://github.com/OasisLMF/OasisLMF/pull/1481) - Set ktools to 3.12.1
+* [#1461](https://github.com/OasisLMF/OasisLMF/pull/1461) - Release 2.3.1
+* [#1464](https://github.com/OasisLMF/OasisLMF/pull/1464) - Feature/add fm tests
+* [#732](https://github.com/OasisLMF/OasisLMF/pull/1465) - Align FM and RI column headers 
+.. _`2.3.2`:  https://github.com/OasisLMF/OasisLMF/compare/2.3.1...2.3.2
+
 `2.3.1`_
  ---------
 * [#1444](https://github.com/OasisLMF/OasisLMF/pull/1444) - support for pandas 3
 * [#1446](https://github.com/OasisLMF/OasisLMF/pull/1446) - Add missing loc_id check
 * [#1447](https://github.com/OasisLMF/OasisLMF/pull/1447) - use correct error_model in back allocation
 * [#1448](https://github.com/OasisLMF/OasisLMF/pull/1448) - ensure header is written in keys.csv
 * [#1449](https://github.com/OasisLMF/OasisLMF/pull/1450) - Footprint_set option not working with parquet format
```

### Comparing `oasislmf-2.3.2/LICENSE` & `oasislmf-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/PKG-INFO` & `oasislmf-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasislmf
-Version: 2.3.2
+Version: 2.3.4
 Summary: Core loss modelling framework.
 Home-page: https://github.com/OasisLMF/oasislmf
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: BSD 3-Clause
 Keywords: oasis lmf loss modeling framework
 Platform: UNKNOWN
```

### Comparing `oasislmf-2.3.2/README.md` & `oasislmf-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/bin/completer_oasislmf` & `oasislmf-2.3.4/bin/completer_oasislmf`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/bin/ktools_monitor.sh` & `oasislmf-2.3.4/bin/ktools_monitor.sh`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/__init__.py` & `oasislmf-2.3.4/oasislmf/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.3.2'
+__version__ = '2.3.4'
 
 import sys
 from importlib.abc import MetaPathFinder, Loader
 from importlib.util import spec_from_loader
 import importlib
 import warnings
```

### Comparing `oasislmf-2.3.2/oasislmf/_data/analysis_settings.json` & `oasislmf-2.3.4/oasislmf/_data/analysis_settings.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/calc_rules_direct.csv` & `oasislmf-2.3.4/oasislmf/_data/calc_rules_direct.csv`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/calc_rules_step.csv` & `oasislmf-2.3.4/oasislmf/_data/calc_rules_step.csv`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/config_compatibility_profile.json` & `oasislmf-2.3.4/oasislmf/_data/config_compatibility_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/default_acc_profile.json` & `oasislmf-2.3.4/oasislmf/_data/default_acc_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/default_combined_exposure_profile.json` & `oasislmf-2.3.4/oasislmf/_data/default_combined_exposure_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/default_fm_agg_profile.json` & `oasislmf-2.3.4/oasislmf/_data/default_fm_agg_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/default_fm_profile_field_values.json` & `oasislmf-2.3.4/oasislmf/_data/default_fm_profile_field_values.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/default_loc_profile.json` & `oasislmf-2.3.4/oasislmf/_data/default_loc_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/_data/default_step_policies_profile.json` & `oasislmf-2.3.4/oasislmf/_data/default_step_policies_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/admin.py` & `oasislmf-2.3.4/oasislmf/cli/admin.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/api.py` & `oasislmf-2.3.4/oasislmf/cli/api.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/command.py` & `oasislmf-2.3.4/oasislmf/cli/command.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/config.py` & `oasislmf-2.3.4/oasislmf/cli/config.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/exposure.py` & `oasislmf-2.3.4/oasislmf/cli/exposure.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/model.py` & `oasislmf-2.3.4/oasislmf/cli/model.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/root.py` & `oasislmf-2.3.4/oasislmf/cli/root.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/cli/test.py` & `oasislmf-2.3.4/oasislmf/cli/test.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/base.py` & `oasislmf-2.3.4/oasislmf/computation/base.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/data/dummy_model/generate.py` & `oasislmf-2.3.4/oasislmf/computation/data/dummy_model/generate.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/generate/files.py` & `oasislmf-2.3.4/oasislmf/computation/generate/files.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/generate/keys.py` & `oasislmf-2.3.4/oasislmf/computation/generate/keys.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/generate/losses.py` & `oasislmf-2.3.4/oasislmf/computation/generate/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,28 @@
 from collections import OrderedDict
 from itertools import product
 from json import JSONDecodeError
 from pathlib import Path
 from subprocess import CalledProcessError, check_call
 
 import pandas as pd
+import numpy as np
 
 from oasis_data_manager.filestore.config import get_storage_from_config_path
+from oasis_data_manager.filestore.backends.local import LocalStorage
+
 from ods_tools.oed.setting_schema import AnalysisSettingSchema, ModelSettingSchema
 
 from ...execution import bash, runner
-from ...execution.bash import get_fmcmd
+from ...execution.bash import get_fmcmd, RUNTYPE_GROUNDUP_LOSS, RUNTYPE_INSURED_LOSS, RUNTYPE_REINSURANCE_LOSS
 from ...execution.bin import (csv_to_bin, prepare_run_directory,
                               prepare_run_inputs, set_footprint_set, set_vulnerability_set)
 from ...preparation.summaries import generate_summaryxref_files
 from ...pytools.fm.financial_structure import create_financial_structure
+from oasislmf.pytools.summary.manager import create_summary_object_file
 from ...utils.data import (fast_zip_dataframe_columns, get_dataframe, get_exposure_data, get_json,
                            get_utctimestamp, merge_dataframes, set_dataframe_column_dtypes)
 from ...utils.defaults import (EVE_DEFAULT_SHUFFLE, EVE_STD_SHUFFLE, KTOOL_N_FM_PER_LB,
                                KTOOL_N_GUL_PER_LB, KTOOLS_ALLOC_FM_MAX, KTOOLS_ALLOC_GUL_DEFAULT,
                                KTOOLS_ALLOC_GUL_MAX, KTOOLS_ALLOC_IL_DEFAULT,
                                KTOOLS_ALLOC_RI_DEFAULT, KTOOLS_DEBUG, KTOOLS_GUL_LEGACY_STREAM,
                                KTOOLS_MEAN_SAMPLE_IDX, KTOOLS_NUM_PROCESSES,
@@ -190,22 +194,39 @@
         {'name': 'ktools_legacy_stream', 'type': str2bool, 'const': True, 'nargs': '?', 'default': KTOOLS_GUL_LEGACY_STREAM,
          'help': 'Run Ground up losses using the older stream type (Compatibility option)'},
         {'name': 'fmpy', 'default': True, 'type': str2bool, 'const': True, 'nargs': '?', 'help': 'use fmcalc python version instead of c++ version'},
         {'name': 'ktools_alloc_rule_il', 'default': KTOOLS_ALLOC_IL_DEFAULT, 'type': int,
          'help': 'Set the fmcalc allocation rule used in direct insured loss'},
         {'name': 'ktools_alloc_rule_ri', 'default': KTOOLS_ALLOC_RI_DEFAULT, 'type': int,
          'help': 'Set the fmcalc allocation rule used in reinsurance'},
+        {'name': 'summarypy', 'default': False, 'type': str2bool, 'const': True,
+            'nargs': '?', 'help': 'use summarycalc python version instead of c++ version'},
         {'name': 'check_missing_inputs', 'default': False, 'type': str2bool, 'const': True, 'nargs': '?',
          'help': 'Fail an analysis run if IL/RI is requested without the required generated files.'},
 
         # Manager only options (pass data directy instead of filepaths)
         {'name': 'verbose', 'default': KTOOLS_DEBUG},
 
     ]
 
+    def _get_storage_manager(self):
+        model_storage = get_storage_from_config_path(
+            self.model_storage_json,
+            os.path.join(self.model_run_dir, "static"),
+        )
+
+        # if not local test the connection to remote storage FS
+        if not isinstance(model_storage, LocalStorage):
+            try:
+                model_storage.listdir()
+            except Exception as e:
+                raise OasisException('Error: Storage Manager connection issue', e)
+
+        return model_storage
+
     def __check_for_parquet_output(self, analysis_settings, runtypes):
         """
         Private method to check whether ktools components were linked to third
         party parquet libraries during compilation if user requests parquet
         output.
         """
         for runtype in runtypes:
@@ -223,19 +244,15 @@
                         )
                     return  # Only need to find a single request
 
     def run(self):
         # need to load from exposure data info or recreate it
         model_run_fp = self._get_output_dir()
         analysis_settings = AnalysisSettingSchema().get(self.analysis_settings_json)
-
-        model_storage = get_storage_from_config_path(
-            self.model_storage_json,
-            os.path.join(self.model_run_dir, "static"),
-        )
+        model_storage = self._get_storage_manager()
 
         il = all(p in os.listdir(self.oasis_files_dir) for p in [
             'fm_policytc.csv',
             'fm_profile.csv',
             'fm_programme.csv',
             'fm_xref.csv'])
 
@@ -338,14 +355,28 @@
 
         if ri and self.fmpy:
             for ri_sub_dir in ri_dirs:
                 ri_target_dir = os.path.join(self.model_run_dir, ri_sub_dir)
                 self.logger.info(f'Creating FMPY structures (RI): {ri_target_dir}')
                 create_financial_structure(self.ktools_alloc_rule_ri, ri_target_dir)
 
+        if self.summarypy:
+            for runtype in [RUNTYPE_GROUNDUP_LOSS, RUNTYPE_INSURED_LOSS, RUNTYPE_REINSURANCE_LOSS]:
+                if analysis_settings.get(f'{runtype}_output'):
+                    summaries = analysis_settings.get('{}_summaries'.format(runtype), [])
+                    summary_sets_id = np.sort([summary['id'] for summary in summaries if 'id' in summary])
+                    if summary_sets_id.shape[0]:
+                        if runtype == RUNTYPE_REINSURANCE_LOSS:
+                            summary_dirs = [os.path.join(self.model_run_dir, ri_sub_dir) for ri_sub_dir in ri_dirs]
+                        else:
+                            summary_dirs = [os.path.join(self.model_run_dir, 'input')]
+                        for summary_dir in summary_dirs:
+                            self.logger.info(f'Creating summarypy structures {runtype}: {summary_dir}')
+                            create_summary_object_file(summary_dir, runtype)
+
         self._store_run_settings(analysis_settings, os.path.join(model_run_fp, 'output'))
         return analysis_settings
 
 
 class GenerateLossesPartial(GenerateLossesDir):
     """
     Runs a single analysis event chunk
@@ -383,14 +414,16 @@
          'help': 'Size in MB of the cache for the vulnerability calculations. Default: 200'},
         {'name': 'fmpy', 'default': True, 'type': str2bool, 'const': True, 'nargs': '?', 'help': 'use fmcalc python version instead of c++ version'},
         {'name': 'fmpy_low_memory', 'default': False, 'type': str2bool, 'const': True, 'nargs': '?',
          'help': 'use memory map instead of RAM to store loss array (may decrease performance but reduce RAM usage drastically)'},
         {'name': 'fmpy_sort_output', 'default': False, 'type': str2bool, 'const': True, 'nargs': '?', 'help': 'order fmpy output by item_id'},
         {'name': 'model_custom_gulcalc', 'default': None, 'help': 'Custom gulcalc binary name to call in the model losses step'},
         {'name': 'peril_filter', 'default': [], 'nargs': '+', 'help': 'Peril specific run'},
+        {'name': 'summarypy', 'default': False, 'type': str2bool, 'const': True,
+            'nargs': '?', 'help': 'use summarycalc python version instead of c++ version'},
         {'name': 'base_df_engine', 'default': "oasis_data_manager.df_reader.reader.OasisPandasReader", 'help': 'The engine to use when loading dataframes'},
         {'name': 'exposure_df_engine', 'default': None,
             'help': 'The engine to use when loading dataframes exposure data (default: same as --base-df-engine)'},
         {'name': 'model_df_engine', 'default': None,
             'help': 'The engine to use when loading dataframes model data (default: same as --base-df-engine)'},
 
         # New vars for chunked loss generation
@@ -445,14 +478,15 @@
             fmpy_low_memory=self.fmpy_low_memory,
             fmpy_sort_output=self.fmpy_sort_output,
             event_shuffle=self.ktools_event_shuffle,
             process_number=self.process_number,
             max_process_id=self.max_process_id,
             modelpy=self.modelpy,
             peril_filter=self._get_peril_filter(self.analysis_settings),
+            summarypy=self.summarypy,
             exposure_df_engine=self.exposure_df_engine or self.base_df_engine,
             model_df_engine=self.model_df_engine or self.base_df_engine,
         )
         # Workaround test -- needs adding into bash_params
         if self.ktools_fifo_queue_dir:
             bash_params['fifo_queue_dir'] = self.ktools_fifo_queue_dir
 
@@ -596,14 +630,16 @@
         {'name': 'fmpy', 'default': True, 'type': str2bool, 'const': True, 'nargs': '?', 'help': 'use fmcalc python version instead of c++ version'},
         {'name': 'fmpy_low_memory', 'default': False, 'type': str2bool, 'const': True, 'nargs': '?',
          'help': 'use memory map instead of RAM to store loss array (may decrease performance but reduce RAM usage drastically)'},
         {'name': 'fmpy_sort_output', 'default': False, 'type': str2bool, 'const': True, 'nargs': '?', 'help': 'order fmpy output by item_id'},
         {'name': 'model_custom_gulcalc', 'default': None, 'help': 'Custom gulcalc binary name to call in the model losses step'},
         {'name': 'model_py_server', 'default': False, 'type': str2bool, 'help': 'running the data server for modelpy'},
         {'name': 'peril_filter', 'default': [], 'nargs': '+', 'help': 'Peril specific run'},
+        {'name': 'summarypy', 'default': False, 'type': str2bool, 'const': True,
+            'nargs': '?', 'help': 'use summarycalc python version instead of c++ version'},
         {'name': 'model_custom_gulcalc_log_start', 'default': None, 'help': 'Log message produced when custom gulcalc binary process starts'},
         {'name': 'model_custom_gulcalc_log_finish', 'default': None, 'help': 'Log message produced when custom gulcalc binary process ends'},
         {'name': 'base_df_engine', 'default': "oasis_data_manager.df_reader.reader.OasisPandasReader", 'help': 'The engine to use when loading dataframes'},
         {'name': 'model_df_engine', 'default': None,
             'help': 'The engine to use when loading model data dataframes (default: --base-df-engine if not set)'},
         {'name': 'exposure_df_engine', 'default': None,
             'help': 'The engine to use when loading exposure data dataframes (default: --base-df-engine if not set)'},
@@ -647,14 +683,15 @@
                         fmpy=self.fmpy,
                         fmpy_low_memory=self.fmpy_low_memory,
                         fmpy_sort_output=self.fmpy_sort_output,
                         event_shuffle=self.ktools_event_shuffle,
                         modelpy=self.modelpy,
                         model_py_server=self.model_py_server,
                         peril_filter=self._get_peril_filter(analysis_settings),
+                        summarypy=self.summarypy,
                         model_df_engine=self.model_df_engine or self.base_df_engine,
                     )
                 except TypeError:
                     warnings.simplefilter("always")
                     warnings.warn(
                         f"{package_name}.supplier_model_runner doesn't accept new runner arguments, please add **kwargs to the run function signature")
                     model_runner_module.run(
```

### Comparing `oasislmf-2.3.2/oasislmf/computation/helper/autocomplete.py` & `oasislmf-2.3.4/oasislmf/computation/helper/autocomplete.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/hooks/post_analysis.py` & `oasislmf-2.3.4/oasislmf/computation/hooks/post_analysis.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/hooks/pre_analysis.py` & `oasislmf-2.3.4/oasislmf/computation/hooks/pre_analysis.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/run/exposure.py` & `oasislmf-2.3.4/oasislmf/computation/run/exposure.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/run/generate_files.py` & `oasislmf-2.3.4/oasislmf/computation/run/generate_files.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/run/generate_losses.py` & `oasislmf-2.3.4/oasislmf/computation/run/generate_losses.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/run/model.py` & `oasislmf-2.3.4/oasislmf/computation/run/model.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/computation/run/platform.py` & `oasislmf-2.3.4/oasislmf/computation/run/platform.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/execution/bash.py` & `oasislmf-2.3.4/oasislmf/execution/bash.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     Args:
         custom_gulcalc_log_start (str): Custom message printed to the logs when a process starts.
         custom_gulcalc_log_finish (str): Custom message printed to the logs when a process ends.
     """
     check_function = """
 check_complete(){
     set +e
-    proc_list="eve getmodel gulcalc fmcalc summarycalc eltcalc aalcalc aalcalcmeanonly leccalc pltcalc ordleccalc modelpy gulpy fmpy gulmc"
+    proc_list="eve getmodel gulcalc fmcalc summarycalc eltcalc aalcalc aalcalcmeanonly leccalc pltcalc ordleccalc modelpy gulpy fmpy gulmc summarypy"
     has_error=0
     for p in $proc_list; do
         started=$(find log -name "${p}_[0-9]*.log" | wc -l)
         finished=$(find log -name "${p}_[0-9]*.log" -exec grep -l "finish" {} + | wc -l)
         if [ "$finished" -lt "$started" ]; then
             echo "[ERROR] $p - $((started-finished)) processes lost"
             has_error=1
@@ -836,37 +836,41 @@
 
 
 def do_summarycalcs(
     runtype,
     analysis_settings,
     process_id,
     filename,
+    summarypy,
     fifo_dir='fifo/',
     stderr_guard=True,
     num_reinsurance_iterations=0,
     gul_legacy_stream=None,
     gul_full_correlation=False,
-    ri_inuring_priority=None
+    ri_inuring_priority=None,
 ):
 
     summaries = analysis_settings.get('{}_summaries'.format(runtype))
     if not summaries:
         return
 
     if process_id == 1:
         print_command(filename, '')
 
-    summarycalc_switch = '-f'
-    if runtype == RUNTYPE_GROUNDUP_LOSS:
-        if gul_legacy_stream:
-            # gul coverage stream
-            summarycalc_switch = '-g'
-        else:
-            # Accept item stream only
-            summarycalc_switch = '-i'
+    if summarypy:
+        summarycalc_switch = f'-t {runtype}'
+    else:
+        summarycalc_switch = '-f'
+        if runtype == RUNTYPE_GROUNDUP_LOSS:
+            if gul_legacy_stream:
+                # gul coverage stream
+                summarycalc_switch = '-g'
+            else:
+                # Accept item stream only
+                summarycalc_switch = '-i'
 
     summarycalc_directory_switch = ""
     inuring_priority_text = ''   # Only relevant for reinsurance
     if runtype == RUNTYPE_REINSURANCE_LOSS:
         if ri_inuring_priority['level']:
             summarycalc_directory_switch = f'-p RI_{ri_inuring_priority["level"]}'
             inuring_priority_text = ri_inuring_priority['text']
@@ -877,15 +881,16 @@
 
     input_filename_component = ''
     if gul_full_correlation:
         input_filename_component = '_sumcalc'
 
     # Use -m flag to create summary index files
     # This is likely to become default in future ktools releases
-    cmd = 'summarycalc -m {} {}'.format(summarycalc_switch, summarycalc_directory_switch)
+    cmd = 'summarypy' if summarypy else 'summarycalc'
+    cmd = f'{cmd} -m {summarycalc_switch} {summarycalc_directory_switch}'
     for summary in summaries:
         if 'id' in summary:
             summary_set = summary['id']
             cmd = '{0} -{1} {4}{2}_{5}S{1}_summary_P{3}'.format(
                 cmd, summary_set, runtype, process_id, fifo_dir,
                 inuring_priority_text
             )
@@ -1134,14 +1139,15 @@
 
 def ri(
     analysis_settings,
     max_process_id,
     filename,
     process_counter,
     num_reinsurance_iterations,
+    summarypy,
     fifo_dir='fifo/',
     work_dir='work/',
     stderr_guard=True,
     process_number=None
 ):
 
     for inuring_priority in get_ri_inuring_priorities(analysis_settings):
@@ -1166,51 +1172,54 @@
                 ri_inuring_priority=inuring_priority['text']
             )
 
         # TODO => insert server here
 
         for process_id in process_range(max_process_id, process_number):
             do_summarycalcs(
+                summarypy=summarypy,
                 runtype=RUNTYPE_REINSURANCE_LOSS,
                 analysis_settings=analysis_settings,
                 process_id=process_id,
                 filename=filename,
                 fifo_dir=fifo_dir,
                 stderr_guard=stderr_guard,
                 num_reinsurance_iterations=num_reinsurance_iterations,
                 ri_inuring_priority=inuring_priority
             )
 
 
-def il(analysis_settings, max_process_id, filename, process_counter, fifo_dir='fifo/', work_dir='work/', stderr_guard=True, process_number=None):
+def il(analysis_settings, max_process_id, filename, process_counter, summarypy, fifo_dir='fifo/', work_dir='work/', stderr_guard=True, process_number=None):
     for process_id in process_range(max_process_id, process_number):
         do_any(RUNTYPE_INSURED_LOSS, analysis_settings, process_id, filename, process_counter, fifo_dir, work_dir, stderr_guard)
 
     for process_id in process_range(max_process_id, process_number):
         do_ord(RUNTYPE_INSURED_LOSS, analysis_settings, process_id, filename, process_counter, fifo_dir, work_dir, stderr_guard)
 
     for process_id in process_range(max_process_id, process_number):
         do_tees(RUNTYPE_INSURED_LOSS, analysis_settings, process_id, filename, process_counter, fifo_dir, work_dir)
 
     for process_id in process_range(max_process_id, process_number):
         do_summarycalcs(
+            summarypy=summarypy,
             runtype=RUNTYPE_INSURED_LOSS,
             analysis_settings=analysis_settings,
             process_id=process_id,
             filename=filename,
             fifo_dir=fifo_dir,
             stderr_guard=stderr_guard,
         )
 
 
 def do_gul(
     analysis_settings,
     max_process_id,
     filename,
     process_counter,
+    summarypy,
     fifo_dir='fifo/',
     work_dir='work/',
     gul_legacy_stream=None,
     stderr_guard=True,
     process_number=None,
 ):
 
@@ -1221,14 +1230,15 @@
         do_ord(RUNTYPE_GROUNDUP_LOSS, analysis_settings, process_id, filename, process_counter, fifo_dir, work_dir, stderr_guard)
 
     for process_id in process_range(max_process_id, process_number):
         do_tees(RUNTYPE_GROUNDUP_LOSS, analysis_settings, process_id, filename, process_counter, fifo_dir, work_dir)
 
     for process_id in process_range(max_process_id, process_number):
         do_summarycalcs(
+            summarypy=summarypy,
             runtype=RUNTYPE_GROUNDUP_LOSS,
             analysis_settings=analysis_settings,
             process_id=process_id,
             filename=filename,
             gul_legacy_stream=gul_legacy_stream,
             fifo_dir=fifo_dir,
             stderr_guard=stderr_guard
@@ -1752,14 +1762,15 @@
     gulmc_vuln_cache_size=200,
 
     # new options
     process_number=None,
     remove_working_files=True,
     model_run_dir='',
     model_py_server=False,
+    summarypy=False,
     peril_filter=[],
     exposure_df_engine="oasis_data_manager.df_reader.reader.OasisPandasReader",
     model_df_engine="oasis_data_manager.df_reader.reader.OasisPandasReader",
     **kwargs
 ):
 
     bash_params = {}
@@ -1790,14 +1801,15 @@
         bash_params['model_storage_json'] = model_storage_json
 
     bash_params['gul_threshold'] = analysis_settings.get('gul_threshold', 0)
     bash_params['number_of_samples'] = analysis_settings.get('number_of_samples', 0)
     bash_params["static_path"] = os.path.join(model_run_dir, "static/")
 
     bash_params["model_py_server"] = model_py_server
+    bash_params['summarypy'] = summarypy if not gul_legacy_stream else False  # summarypy doesn't support gul_legacy_stream
     bash_params["peril_filter"] = peril_filter
 
     # set complex model gulcalc command
     if not _get_getmodel_cmd and custom_gulcalc_cmd:
         bash_params['_get_getmodel_cmd'] = get_complex_model_cmd(custom_gulcalc_cmd, analysis_settings)
     else:
         bash_params['_get_getmodel_cmd'] = _get_getmodel_cmd
@@ -2000,14 +2012,15 @@
     gulpy_random_generator,
     gulmc,
     gulmc_random_generator,
     gulmc_effective_damageability,
     gulmc_vuln_cache_size,
     model_py_server,
     peril_filter,
+    summarypy,
     gul_legacy_stream=False,
     model_df_engine='oasis_data_manager.df_reader.reader.OasisPandasReader',
     **kwargs
 ):
 
     process_counter = process_counter or Counter()
     custom_args = custom_args or {}
@@ -2167,14 +2180,15 @@
                 'loss_type': 'reinsurance',
                 'compute_fun': ri,
                 'compute_args': {
                     'analysis_settings': analysis_settings,
                     'max_process_id': num_fm_output,
                     'filename': filename,
                     'process_counter': process_counter,
+                    'summarypy': summarypy,
                     'num_reinsurance_iterations': num_reinsurance_iterations,
                     'fifo_dir': _fifo_dir,
                     'work_dir': _work_dir,
                     'stderr_guard': stderr_guard,
                     'process_number': process_number
                 }
             }
@@ -2185,14 +2199,15 @@
                 'loss_type': 'insured',
                 'compute_fun': il,
                 'compute_args': {
                     'analysis_settings': analysis_settings,
                     'max_process_id': num_fm_output,
                     'filename': filename,
                     'process_counter': process_counter,
+                    'summarypy': summarypy,
                     'fifo_dir': _fifo_dir,
                     'work_dir': _work_dir,
                     'stderr_guard': stderr_guard,
                     'process_number': process_number
                 }
             }
             compute_outputs.append(il_computes)
@@ -2202,14 +2217,15 @@
                 'loss_type': 'ground up',
                 'compute_fun': do_gul,
                 'compute_args': {
                     'analysis_settings': analysis_settings,
                     'max_process_id': num_gul_output,
                     'filename': filename,
                     'process_counter': process_counter,
+                    'summarypy': summarypy,
                     'fifo_dir': _fifo_dir,
                     'work_dir': _work_dir,
                     'gul_legacy_stream': gul_legacy_stream,
                     'stderr_guard': stderr_guard,
                     'process_number': process_number
                 }
             }
@@ -2601,14 +2617,15 @@
     gulpy_random_generator=1,
     gulmc=False,
     gulmc_random_generator=1,
     gulmc_effective_damageability=False,
     gulmc_vuln_cache_size=200,
     model_py_server=False,
     peril_filter=[],
+    summarypy=False,
     base_df_engine='oasis_data_manager.df_reader.reader.OasisPandasReader',
     model_df_engine=None,
 ):
     """
     Generates a bash script containing ktools calculation instructions for an
     Oasis model.
 
@@ -2682,14 +2699,15 @@
         gulpy_random_generator=gulpy_random_generator,
         gulmc=gulmc,
         gulmc_random_generator=gulmc_random_generator,
         gulmc_effective_damageability=gulmc_effective_damageability,
         gulmc_vuln_cache_size=gulmc_vuln_cache_size,
         model_py_server=model_py_server,
         peril_filter=peril_filter,
+        summarypy=summarypy,
         model_df_engine=model_df_engine,
     )
 
     # remove the file if it already exists
     if os.path.exists(filename):
         os.remove(filename)
```

### Comparing `oasislmf-2.3.2/oasislmf/execution/bin.py` & `oasislmf-2.3.4/oasislmf/execution/bin.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,15 @@
 
 from oasis_data_manager.filestore.backends.base import BaseStorage
 from ..utils.exceptions import OasisException
 from ..utils.log import oasis_log
 from ..utils.defaults import STATIC_DATA_FP
 from .files import TAR_FILE, INPUT_FILES, GUL_INPUT_FILES, IL_INPUT_FILES
 from .bash import leccalc_enabled, ord_enabled, ORD_LECCALC
-from oasislmf.pytools.getmodel.common import fp_format_priorities
-from oasislmf.pytools.getmodel.footprint import (
-    FootprintParquet, FootprintBinZ, FootprintBin, FootprintCsv
-)
+from oasislmf.pytools.getmodel.footprint import Footprint
 from oasislmf.pytools.getmodel.vulnerability import vulnerability_dataset, parquetvulnerability_meta_filename
 
 logger = logging.getLogger(__name__)
 
 
 @oasis_log
 def prepare_run_directory(
@@ -203,15 +200,18 @@
                 else:
                     # If the link already exists, check files are different replace it
                     if os.readlink(destfile) != os.path.abspath(sourcefile):
                         os.symlink(sourcefile, destfile + ".tmp")
                         os.replace(destfile + ".tmp", destfile)
 
         if model_storage_config_fp:
-            shutil.copy(model_storage_config_fp, os.path.join(run_dir, "model_storage.json"))
+            try:
+                shutil.copy(model_storage_config_fp, os.path.join(run_dir, "model_storage.json"))
+            except shutil.SameFileError as e:
+                pass
 
         if user_data_dir and os.path.exists(user_data_dir):
             for sourcefile in glob.glob(os.path.join(user_data_dir, '*')):
                 destfile = os.path.join(model_data_dst_fp, os.path.basename(sourcefile))
 
                 try:
                     if os.name == 'nt':
@@ -296,27 +296,17 @@
         else:
             targets = [
                 f"{bin_name}_{str(setting_val)}.{extension}",
                 f"{bin_name}_{str(setting_val).replace(' ', '_').lower()}.{extension}"
             ]
 
         for fname in targets:
-            if storage.isfile(fname):
+            if storage.exists(fname):
                 storage.get(fname, bin_fp)
 
-        # if not setting_val:
-        #     model_data_bin_fp = os.path.join(run_dir, 'static', '{}.{}'.format(bin_name, extension))
-        # else:
-        #     # 'verbatim' -  Try setting value as given
-        #     model_data_bin_fp = os.path.join(run_dir, 'static', '{}_{}.{}'.format(bin_name, str(setting_val), extension))
-        #     if not os.path.isfile(model_data_bin_fp):
-        #         # 'compatibility' - Fallback name formatting to keep existing conversion
-        #         setting_val = str(setting_val).replace(' ', '_').lower()
-        #         model_data_bin_fp = os.path.join(run_dir, 'static', '{}_{}.{}'.format(bin_name, setting_val, extension))
-
         if not os.path.exists(bin_fp):
             raise OasisException('Could not find {} data file: {}'.format(bin_name, targets))
 
 
 def _calc_selected(analysis_settings, calc_type_list):
     """
     Return True, if any options in "calc_type_list" are set in the analysis settings file
@@ -432,19 +422,15 @@
 
     :param setting_val: identifier for footprint set
     :type setting_val: string
 
     :param run_dir: model run directory
     :type run_dir: string
     """
-    format_to_class = {
-        'parquet': FootprintParquet, 'binZ': FootprintBinZ,
-        'bin': FootprintBin, 'csv': FootprintCsv
-    }
-    priorities = [format_to_class[fmt] for fmt in fp_format_priorities if fmt in format_to_class]
+    priorities = Footprint.get_footprint_fmt_priorities()
     setting_val = str(setting_val)
 
     for footprint_class in priorities:
         for filename in footprint_class.footprint_filenames:
             stem, extension = filename.split('.', 1)
             footprint_fp = os.path.join(run_dir, 'static', f'{stem}_{setting_val}.{extension}')
             footprint_target_fp = os.path.join(run_dir, 'static', filename)
```

### Comparing `oasislmf-2.3.2/oasislmf/execution/complex_items_to_bin.py` & `oasislmf-2.3.4/oasislmf/execution/complex_items_to_bin.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/execution/complex_items_to_csv.py` & `oasislmf-2.3.4/oasislmf/execution/complex_items_to_csv.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/execution/conf.py` & `oasislmf-2.3.4/oasislmf/execution/conf.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/execution/files.py` & `oasislmf-2.3.4/oasislmf/execution/files.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/execution/load_balancer.py` & `oasislmf-2.3.4/oasislmf/execution/load_balancer.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/execution/runner.py` & `oasislmf-2.3.4/oasislmf/execution/runner.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/lookup/base.py` & `oasislmf-2.3.4/oasislmf/lookup/base.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/lookup/builtin.py` & `oasislmf-2.3.4/oasislmf/lookup/builtin.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/lookup/factory.py` & `oasislmf-2.3.4/oasislmf/lookup/factory.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/lookup/interface.py` & `oasislmf-2.3.4/oasislmf/lookup/interface.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/manager.py` & `oasislmf-2.3.4/oasislmf/manager.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/platform_api/client.py` & `oasislmf-2.3.4/oasislmf/platform_api/client.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/platform_api/session.py` & `oasislmf-2.3.4/oasislmf/platform_api/session.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/preparation/correlations.py` & `oasislmf-2.3.4/oasislmf/preparation/correlations.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/preparation/dir_inputs.py` & `oasislmf-2.3.4/oasislmf/preparation/dir_inputs.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/preparation/gul_inputs.py` & `oasislmf-2.3.4/oasislmf/preparation/gul_inputs.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/preparation/il_inputs.py` & `oasislmf-2.3.4/oasislmf/preparation/il_inputs.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/preparation/oed.py` & `oasislmf-2.3.4/oasislmf/preparation/oed.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/preparation/reinsurance_layer.py` & `oasislmf-2.3.4/oasislmf/preparation/reinsurance_layer.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/preparation/summaries.py` & `oasislmf-2.3.4/oasislmf/preparation/summaries.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/cdftocsv.py` & `oasislmf-2.3.4/oasislmf/pytools/cdftocsv.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/correlationtobin.py` & `oasislmf-2.3.4/oasislmf/pytools/correlationtobin.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/correlationtocsv.py` & `oasislmf-2.3.4/oasislmf/pytools/correlationtocsv.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/data_layer/conversions/correlations.py` & `oasislmf-2.3.4/oasislmf/pytools/data_layer/conversions/correlations.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/data_layer/conversions/footprint.py` & `oasislmf-2.3.4/oasislmf/pytools/data_layer/conversions/footprint.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/data_layer/footprint_layer.py` & `oasislmf-2.3.4/oasislmf/pytools/data_layer/footprint_layer.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/data_layer/oasis_files/correlations.py` & `oasislmf-2.3.4/oasislmf/pytools/data_layer/oasis_files/correlations.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from typing import Optional
 
 import numba as nb
 import numpy as np
 import pandas as pd
 
-from oasislmf.pytools.common import oasis_float
+from oasislmf.pytools.common.data import oasis_float
 
 logger = logging.getLogger(__name__)
 
 
 Correlation = nb.from_dtype(np.dtype([
     ('item_id', np.int32),
     ("peril_correlation_group", np.int32),
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/dfcompare.py` & `oasislmf-2.3.4/oasislmf/pytools/dfcompare.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/back_allocation.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/back_allocation.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/compare.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from numpy.testing import assert_allclose
-from .stream import event_agg_dtype, sidx_loss_dtype, EXTRA_VALUES
-from .common import np_oasis_float
+from oasislmf.pytools.common.data import oasis_float
+from .stream_sparse import event_agg_dtype, sidx_loss_dtype
+from .common import EXTRA_VALUES
 from .financial_structure import load_static
 
 
 def stream_to_dict_array(stream_obj):
     stream_type = stream_obj.read(4)
     len_sample = np.frombuffer(stream_obj.read(4), dtype=np.int32)[0]
 
@@ -32,15 +33,15 @@
         else:
             event_id, agg_id = event_agg[0]
             # if event_id_last != event_id:
             #     if event_id_last:
             #         break
             #     else:
             #         event_id_last = event_id
-            cur_array = np.zeros(len_sample + EXTRA_VALUES, dtype=np_oasis_float)
+            cur_array = np.zeros(len_sample + EXTRA_VALUES, dtype=oasis_float)
             dict_array[(event_id, agg_id)] = cur_array
 
     return stream_type, len_sample, dict_array
 
 
 def round_dict_array(dict_array, precision):
     for key, values in dict_array.items():
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/compute_sparse.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/compute_sparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from oasislmf.pytools.common.data import oasis_float, oasis_int, null_index
 from .policy import calc
 from .policy_extras import calc as calc_extra
-from .common import np_oasis_float, np_oasis_int, EXTRA_VALUES, null_index, compute_idx_dtype, DEDUCTIBLE, UNDERLIMIT, OVERLIMIT
+from .common import EXTRA_VALUES, compute_idx_dtype, DEDUCTIBLE, UNDERLIMIT, OVERLIMIT
 from .back_allocation import back_alloc_a2, back_alloc_extra_a2, back_alloc_layer, back_alloc_layer_extra
 
 from numba import njit
 import numpy as np
 import os
 import logging
 logger = logging.getLogger(__name__)
@@ -344,42 +345,42 @@
     """
     compute_idx['sidx_i'] = compute_idx['next_compute_i']
     compute_idx['sidx_ptr_i'] = compute_idx['loss_ptr_i'] = sidx_indptr[compute_idx['next_compute_i']]
     compute_idx['extras_ptr_i'] = 0
     compute_idx['compute_i'] = 0
 
     # dense array to store if sample id has value for this node
-    temp_node_sidx = np.zeros(len_array, dtype=np_oasis_int)
+    temp_node_sidx = np.zeros(len_array, dtype=oasis_int)
 
     # sparse array to store the loss after profile is applied
-    temp_node_loss_sparse = np.zeros(len_array, dtype=np_oasis_float)
+    temp_node_loss_sparse = np.zeros(len_array, dtype=oasis_float)
 
     # sparse array to store the merged loss of all layer
-    temp_node_loss_layer_merge = np.zeros(len_array, dtype=np_oasis_float)
+    temp_node_loss_layer_merge = np.zeros(len_array, dtype=oasis_float)
 
     # sparse array to loss after layer back alloc
-    temp_node_loss_layer_ba = np.zeros((compute_info['max_layer'], len_array), dtype=np_oasis_float)
+    temp_node_loss_layer_ba = np.zeros((compute_info['max_layer'], len_array), dtype=oasis_float)
 
     # temp_node_loss: dense array storing the sum of children loss, then the loss factor in children back alloc
     temp_node_loss = np.zeros((compute_info['max_layer'], len_array), dtype=np.float64)
 
     # temp_node_extras: dense array storing the sum of children extra, then the loss factor in children back alloc
-    temp_node_extras = np.zeros((compute_info['max_layer'], len_array, 3), dtype=np_oasis_float)
+    temp_node_extras = np.zeros((compute_info['max_layer'], len_array, 3), dtype=oasis_float)
 
     # temp_node_extras_layer_merge: sparse array to store the merged extra of all layer
-    temp_node_extras_layer_merge = np.zeros((len_array, 3), dtype=np_oasis_float)
+    temp_node_extras_layer_merge = np.zeros((len_array, 3), dtype=oasis_float)
 
     # temp_node_extras_layer_merge_save: sparse array to keep the value of extra when profile is apply on merged layer
-    temp_node_extras_layer_merge_save = np.zeros((len_array, 3), dtype=np_oasis_float)
+    temp_node_extras_layer_merge_save = np.zeros((len_array, 3), dtype=oasis_float)
 
     # temp_children_queue: array storing all the base children of the node
-    temp_children_queue = np.empty(nodes_array.shape[0], dtype=np_oasis_int)
+    temp_children_queue = np.empty(nodes_array.shape[0], dtype=oasis_int)
 
     # create all sidx array
-    all_sidx = np.empty(max_sidx_val + EXTRA_VALUES, dtype=np_oasis_int)
+    all_sidx = np.empty(max_sidx_val + EXTRA_VALUES, dtype=oasis_int)
     all_sidx[0] = -5
     all_sidx[1] = -3
     all_sidx[2] = -1
     all_sidx[3:] = np.arange(1, max_sidx_val + 1)
 
     is_allocation_rule_a0 = compute_info['allocation_rule'] == 0
     is_allocation_rule_a1 = compute_info['allocation_rule'] == 1
@@ -724,33 +725,33 @@
     therefore we can use only sidx_indexes to tract the length of each node values
     """
     max_sidx_count = max_sidx_val + EXTRA_VALUES
     len_array = max_sidx_val + 6
 
     if low_memory:
         sidx_val = np.memmap(os.path.join(temp_dir, "sidx_val.bin"), mode='w+',
-                             shape=(compute_info['node_len'] * max_sidx_count), dtype=np_oasis_int)
+                             shape=(compute_info['node_len'] * max_sidx_count), dtype=oasis_int)
         loss_val = np.memmap(os.path.join(temp_dir, "loss_val.bin"), mode='w+',
-                             shape=(compute_info['loss_len'] * max_sidx_count), dtype=np_oasis_float)
+                             shape=(compute_info['loss_len'] * max_sidx_count), dtype=oasis_float)
         extras_val = np.memmap(os.path.join(temp_dir, "extras_val.bin"), mode='w+',
-                               shape=(compute_info['extra_len'] * max_sidx_count, 3), dtype=np_oasis_float)
+                               shape=(compute_info['extra_len'] * max_sidx_count, 3), dtype=oasis_float)
     else:
-        sidx_val = np.zeros((compute_info['node_len'] * max_sidx_count), dtype=np_oasis_int)
-        loss_val = np.zeros((compute_info['loss_len'] * max_sidx_count), dtype=np_oasis_float)
-        extras_val = np.zeros((compute_info['extra_len'] * max_sidx_count, 3), dtype=np_oasis_float)
+        sidx_val = np.zeros((compute_info['node_len'] * max_sidx_count), dtype=oasis_int)
+        loss_val = np.zeros((compute_info['loss_len'] * max_sidx_count), dtype=oasis_float)
+        extras_val = np.zeros((compute_info['extra_len'] * max_sidx_count, 3), dtype=oasis_float)
 
     sidx_indptr = np.zeros(compute_info['node_len'] + 1, dtype=np.int64)
     loss_indptr = np.zeros(compute_info['loss_len'] + 1, dtype=np.int64)
     extras_indptr = np.zeros(compute_info['extra_len'] + 1, dtype=np.int64)
 
-    sidx_indexes = np.empty(compute_info['node_len'], dtype=np_oasis_int)
+    sidx_indexes = np.empty(compute_info['node_len'], dtype=oasis_int)
     children = np.zeros(compute_info['children_len'], dtype=np.uint32)
     computes = np.zeros(compute_info['compute_len'], dtype=np.uint32)
 
-    pass_through = np.zeros(compute_info['items_len'] + 1, dtype=np_oasis_float)
+    pass_through = np.zeros(compute_info['items_len'] + 1, dtype=oasis_float)
     item_parent_i = np.ones(compute_info['items_len'] + 1, dtype=np.uint32)
 
     compute_idx = np.empty(1, dtype=compute_idx_dtype)[0]
     compute_idx['next_compute_i'] = 0
 
     return (max_sidx_val, max_sidx_count, len_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val,
             pass_through, extras_indptr, extras_val, children, computes, item_parent_i, compute_idx)
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/financial_structure.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/financial_structure.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,130 +5,106 @@
     'load_static',
 ]
 
 import logging
 import os
 
 import numpy as np
-import pandas as pd
 from numba import from_dtype, njit, types
 from numba.typed import Dict, List
 
-from .common import (allowed_allocation_rule, almost_equal, fm_policytc_dtype,
-                     fm_profile_csv_col_map, fm_profile_dtype,
-                     fm_profile_step_dtype, fm_programme_dtype,
-                     fm_xref_csv_col_map, fm_xref_dtype, items_dtype,
-                     nb_oasis_int, need_extras, need_tiv_policy,
-                     np_oasis_float, np_oasis_int, null_index)
+
+from oasislmf.pytools.common.data import (load_as_ndarray, load_as_array, almost_equal,
+                                          fm_policytc_dtype,
+                                          fm_profile_csv_col_map, fm_profile_dtype, fm_profile_step_dtype,
+                                          fm_programme_dtype,
+                                          fm_xref_csv_col_map, fm_xref_dtype,
+                                          items_dtype,
+                                          oasis_int, nb_oasis_int, oasis_float, null_index)
+from .common import (allowed_allocation_rule, need_extras, need_tiv_policy)
 
 logger = logging.getLogger(__name__)
 
 # temp dictionary types
 node_type = types.UniTuple(nb_oasis_int, 2)
 output_type = types.UniTuple(nb_oasis_int, 2)
 layer_type = types.UniTuple(nb_oasis_int, 3)
 
 # financial structure processed array
 nodes_array_dtype = from_dtype(np.dtype([('node_id', np.uint64),
-                                         ('level_id', np_oasis_int),
-                                         ('agg_id', np_oasis_int),
-                                         ('layer_len', np_oasis_int),
-                                         ('cross_layer_profile', np_oasis_int),
-                                         ('profile_len', np_oasis_int),
-                                         ('profiles', np_oasis_int),
-                                         ('loss', np_oasis_int),
-                                         ('net_loss', np_oasis_int),
-                                         ('extra', np_oasis_int),
+                                         ('level_id', oasis_int),
+                                         ('agg_id', oasis_int),
+                                         ('layer_len', oasis_int),
+                                         ('cross_layer_profile', oasis_int),
+                                         ('profile_len', oasis_int),
+                                         ('profiles', oasis_int),
+                                         ('loss', oasis_int),
+                                         ('net_loss', oasis_int),
+                                         ('extra', oasis_int),
                                          ('is_reallocating', np.uint8),
-                                         ('parent_len', np_oasis_int),
-                                         ('parent', np_oasis_int),
-                                         ('children', np_oasis_int),
-                                         ('output_ids', np_oasis_int),
+                                         ('parent_len', oasis_int),
+                                         ('parent', oasis_int),
+                                         ('children', oasis_int),
+                                         ('output_ids', oasis_int),
                                          ]))
 
-compute_info_dtype = from_dtype(np.dtype([('allocation_rule', np_oasis_int),
-                                          ('max_level', np_oasis_int),
-                                          ('max_layer', np_oasis_int),
-                                          ('node_len', np_oasis_int),
-                                          ('children_len', np_oasis_int),
-                                          ('parents_len', np_oasis_int),
-                                          ('profile_len', np_oasis_int),
-                                          ('loss_len', np_oasis_int),
-                                          ('extra_len', np_oasis_int),
-                                          ('compute_len', np_oasis_int),
-                                          ('start_level', np_oasis_int),
-                                          ('items_len', np_oasis_int),
-                                          ('output_len', np_oasis_int),
+compute_info_dtype = from_dtype(np.dtype([('allocation_rule', oasis_int),
+                                          ('max_level', oasis_int),
+                                          ('max_layer', oasis_int),
+                                          ('node_len', oasis_int),
+                                          ('children_len', oasis_int),
+                                          ('parents_len', oasis_int),
+                                          ('profile_len', oasis_int),
+                                          ('loss_len', oasis_int),
+                                          ('extra_len', oasis_int),
+                                          ('compute_len', oasis_int),
+                                          ('start_level', oasis_int),
+                                          ('items_len', oasis_int),
+                                          ('output_len', oasis_int),
                                           ('stepped', np.bool_),
                                           ]))
-profile_index_dtype = from_dtype(np.dtype([('i_start', np_oasis_int),
-                                           ('i_end', np_oasis_int),
+profile_index_dtype = from_dtype(np.dtype([('i_start', oasis_int),
+                                           ('i_end', oasis_int),
                                            ]))
 
 
 def load_static(static_path):
     """
     Load the raw financial data from static_path as numpy ndarray
     first check if .bin file is present then try .cvs
     try loading profile_step before falling back to normal profile,
 
-    # TODO: handle profile_step
-    # profile_step = load_file('fm_profile_step', fm_profile_step_dtype, must_exist=False)
-    # profile = profile_step if profile_step else load_file('fm_profile', fm_profile_dtype)
-
     :param static_path: str
             static_path
     :return:
         programme : link between nodes
         policytc : info on layer
         profile : policy profile can be profile_step or profile
         xref : node to output_id
+        items : items (item_id and coverage_id mapping)
+        coverages : Tiv value for each coverage id
     :raise:
         FileNotFoundError if one of the static is missing
     """
-    def load_file(name, _dtype, must_exist=True, col_map=None):
-        if os.path.isfile(os.path.join(static_path, name + '.bin')):
-            return np.fromfile(os.path.join(static_path, name + '.bin'), dtype=_dtype)
-        elif must_exist or os.path.isfile(os.path.join(static_path, name + '.csv')):
-            # in csv column cam be out of order and have different name,
-            # we load with pandas and write each column to the ndarray
-            if col_map is None:
-                col_map = {}
-            with open(os.path.join(static_path, name + '.csv')) as file_in:
-                cvs_dtype = {col_map.get(key, key): col_dtype for key, (col_dtype, _) in _dtype.fields.items()}
-                df = pd.read_csv(file_in, delimiter=',', dtype=cvs_dtype)
-                res = np.empty(df.shape[0], dtype=_dtype)
-                for name in _dtype.names:
-                    res[name] = df[col_map.get(name, name)]
-                return res
-
-    programme = load_file('fm_programme', fm_programme_dtype)
-    policytc = load_file('fm_policytc', fm_policytc_dtype)
-    profile = load_file('fm_profile_step', fm_profile_step_dtype, False, col_map=fm_profile_csv_col_map)
-    if profile is None:
-        profile = load_file('fm_profile', fm_profile_dtype, col_map=fm_profile_csv_col_map)
+    programme = load_as_ndarray(static_path, 'fm_programme', fm_programme_dtype)
+    policytc = load_as_ndarray(static_path, 'fm_policytc', fm_policytc_dtype)
+    profile = load_as_ndarray(static_path, 'fm_profile_step', fm_profile_step_dtype, False, col_map=fm_profile_csv_col_map)
+    if len(profile) == 0:
+        profile = load_as_ndarray(static_path, 'fm_profile', fm_profile_dtype, col_map=fm_profile_csv_col_map)
         stepped = None
     else:
         stepped = True
-    xref = load_file('fm_xref', fm_xref_dtype, col_map=fm_xref_csv_col_map)
+    xref = load_as_ndarray(static_path, 'fm_xref', fm_xref_dtype, col_map=fm_xref_csv_col_map)
 
-    try:  # try to load items and coverage if present for TIV base policies (not used in re-insurance)
-        items = load_file('items', items_dtype)[['item_id', 'coverage_id']]
-
-        # coverage has a different structure whether it comes for the csv or the bin file
-        fp = os.path.join(static_path, 'coverages.bin')
-        if os.path.isfile(fp):
-            coverages = np.fromfile(fp, dtype=np_oasis_float)
-        else:
-            fp = os.path.join(static_path, 'coverages.csv')
-            with open(fp) as file_in:
-                coverages = np.loadtxt(file_in, dtype=np_oasis_float, delimiter=',', skiprows=1, usecols=1)
-    except FileNotFoundError:
+    items = load_as_ndarray(static_path, 'items', items_dtype, must_exist=False)[['item_id', 'coverage_id']]
+    coverages = load_as_array(static_path, 'coverages', oasis_float, must_exist=False)
+    if np.unique(items['coverage_id']).shape[0] != coverages.shape[0]:
+        # one of the file is missing we default to empty array
         items = np.empty(0, dtype=items_dtype)
-        coverages = np.empty(0, dtype=np_oasis_float)
+        coverages = np.empty(0, dtype=oasis_float)
 
     return programme, policytc, profile, stepped, xref, items, coverages
 
 
 @njit(cache=True)
 def does_nothing(profile):
     """
@@ -334,27 +310,27 @@
         node_profiles_array:
         output_array:
     """
     ##### profile_id_to_profile_index ####
     # policies may have multiple step, crate a mapping between profile_id and the start and end index in fm_profile file
     max_profile_id = np.max(fm_profile['profile_id'])
     profile_id_to_profile_index = np.empty(max_profile_id + 1, dtype=profile_index_dtype)
-    has_tiv_policy = Dict.empty(np_oasis_int, np_oasis_int)
+    has_tiv_policy = Dict.empty(nb_oasis_int, nb_oasis_int)
     last_profile_id = 0  # real profile_id start at 1
     for i in range(fm_profile.shape[0]):
         if fm_profile[i]['calcrule_id'] in need_tiv_policy:
-            has_tiv_policy[fm_profile[i]['profile_id']] = np_oasis_int(0)
+            has_tiv_policy[fm_profile[i]['profile_id']] = nb_oasis_int(0)
         profile_id_to_profile_index[fm_profile[i]['profile_id']]['i_end'] = i + 1
         if last_profile_id != fm_profile[i]['profile_id']:
             profile_id_to_profile_index[fm_profile[i]['profile_id']]['i_start'] = i
             last_profile_id = fm_profile[i]['profile_id']
 
     # in fm_programme check if multi-peril and get size of each levels
     max_level = np.max(fm_programme['level_id'])
-    level_node_len = np.zeros(max_level + 1, dtype=np_oasis_int)
+    level_node_len = np.zeros(max_level + 1, dtype=oasis_int)
     multi_peril = False
     for i in range(fm_programme.shape[0]):
         programme = fm_programme[i]
         if programme['level_id'] == 1 and programme['from_agg_id'] != programme['to_agg_id']:
             multi_peril = True
         if level_node_len[programme['level_id'] - 1] < programme['from_agg_id']:
             level_node_len[programme['level_id'] - 1] = programme['from_agg_id']
@@ -366,28 +342,28 @@
     # programme_node_to_layers dict of (level_id, agg_id) => list of (layer_id, policy_index_start, policy_index_end)
     # for each policy needing tiv, we duplicate the policy for each node to then later on calculate the % tiv parameters
     programme_node_to_layers = Dict.empty(node_type, List.empty_list(layer_type))
     i_new_fm_profile = fm_profile.shape[0]
     new_fm_profile_list = List.empty_list(np.int64)
     for i in range(fm_policytc.shape[0]):
         policytc = fm_policytc[i]
-        programme_node = (np_oasis_int(policytc['level_id']), np_oasis_int(policytc['agg_id']))
-        i_start = profile_id_to_profile_index[np_oasis_int(policytc['profile_id'])]['i_start']
-        i_end = profile_id_to_profile_index[np_oasis_int(policytc['profile_id'])]['i_end']
+        programme_node = (nb_oasis_int(policytc['level_id']), nb_oasis_int(policytc['agg_id']))
+        i_start = profile_id_to_profile_index[nb_oasis_int(policytc['profile_id'])]['i_start']
+        i_end = profile_id_to_profile_index[nb_oasis_int(policytc['profile_id'])]['i_end']
 
         if policytc['profile_id'] in has_tiv_policy:
             if has_tiv_policy[policytc['profile_id']]:
                 for j in range(i_start, i_end):
                     new_fm_profile_list.append(j)
                 i_start, i_end = i_new_fm_profile, i_new_fm_profile + i_end - i_start
                 i_new_fm_profile = i_end
             else:
-                has_tiv_policy[policytc['profile_id']] = np_oasis_int(1)
+                has_tiv_policy[policytc['profile_id']] = nb_oasis_int(1)
 
-        layer = (np_oasis_int(policytc['layer_id']), np_oasis_int(i_start), np_oasis_int(i_end))
+        layer = (nb_oasis_int(policytc['layer_id']), nb_oasis_int(i_start), nb_oasis_int(i_end))
 
         if programme_node not in programme_node_to_layers:
             _list = List.empty_list(layer_type)
             _list.append(layer)
             programme_node_to_layers[programme_node] = _list
         else:
             programme_node_to_layers[programme_node].append(layer)
@@ -398,74 +374,74 @@
         new_fm_profile[:fm_profile.shape[0]] = fm_profile[:]
         for i in range(i_new_fm_profile - fm_profile.shape[0]):
             new_fm_profile[fm_profile.shape[0] + i] = fm_profile[new_fm_profile_list[i]]
         fm_profile = new_fm_profile
 
     # fm_xref
     if multi_peril:  # if single peril we can skip item level computation (level 0)
-        start_level = np_oasis_int(0)
+        start_level = nb_oasis_int(0)
     else:
-        start_level = np_oasis_int(1)
+        start_level = nb_oasis_int(1)
 
     if start_level == max_level:  # there is only one level we can switch the computation as if it were a0
         allocation_rule = 0
 
     if allocation_rule == 0:
-        out_level = np_oasis_int(max_level)
+        out_level = nb_oasis_int(max_level)
     else:
         out_level = start_level
 
     ##### xref #####
     # create mapping node (level_id, agg_id) => list of (layer_id, output_id)
     node_to_output_id = Dict.empty(node_type, List.empty_list(output_type))
 
     output_len = 0
     for i in range(fm_xref.shape[0]):
         xref = fm_xref[i]
         programme_node = (out_level, xref['agg_id'])
         if output_len < xref['output_id']:
-            output_len = np_oasis_int(xref['output_id'])
+            output_len = nb_oasis_int(xref['output_id'])
 
         if programme_node in node_to_output_id:
-            node_to_output_id[programme_node].append((np_oasis_int(xref['layer_id']), np_oasis_int(xref['output_id'])))
+            node_to_output_id[programme_node].append((nb_oasis_int(xref['layer_id']), nb_oasis_int(xref['output_id'])))
         else:
             _list = List.empty_list(output_type)
-            _list.append((np_oasis_int(xref['layer_id']), np_oasis_int(xref['output_id'])))
+            _list.append((nb_oasis_int(xref['layer_id']), nb_oasis_int(xref['output_id'])))
             node_to_output_id[programme_node] = _list
 
     ##### programme ####
     # node_layers will contain the number of layer for each nodes
-    node_layers = Dict.empty(node_type, np_oasis_int)
-    node_cross_layers = Dict.empty(node_type, np_oasis_int)
+    node_layers = Dict.empty(node_type, nb_oasis_int)
+    node_cross_layers = Dict.empty(node_type, nb_oasis_int)
 
     # fill up node_layers with the number of policies for each node
     for programme in fm_programme:
-        parent = (np_oasis_int(programme['level_id']), np_oasis_int(programme['to_agg_id']))
+        parent = (nb_oasis_int(programme['level_id']), nb_oasis_int(programme['to_agg_id']))
         if parent not in node_layers:
-            node_layers[parent] = np_oasis_int(len(programme_node_to_layers[parent]))
+            node_layers[parent] = nb_oasis_int(len(programme_node_to_layers[parent]))
 
     # create 2 mapping to get the parents and the childs of each nodes
     # update the number of layer for nodes based on the number of layer of their parents
     # go through each level from top to botom
     parent_to_children = Dict.empty(node_type, List.empty_list(node_type))
     child_to_parents = Dict.empty(node_type, List.empty_list(node_type))
 
     children_len = 1
     parents_len = 0
 
     # go through each level from top to botom
     for level in range(max_level, start_level, -1):
         for programme in fm_programme:
             if programme['level_id'] == level:
-                parent = (np_oasis_int(programme['level_id']), np_oasis_int(programme['to_agg_id']))
+                parent = (nb_oasis_int(programme['level_id']), nb_oasis_int(programme['to_agg_id']))
 
                 if programme['from_agg_id'] > 0:  # level of node is programme['level_id'] - 1
-                    child_programme = (np_oasis_int(programme['level_id'] - 1), np_oasis_int(programme['from_agg_id']))
+                    child_programme = (nb_oasis_int(programme['level_id'] - 1), nb_oasis_int(programme['from_agg_id']))
                 else:  # negative agg_id level is item level
-                    child_programme = (start_level, np_oasis_int(-programme['from_agg_id']))
+                    child_programme = (start_level, nb_oasis_int(-programme['from_agg_id']))
 
                 if parent not in parent_to_children:
                     children_len += 2
                     _list = List.empty_list(node_type)
                     _list.append(child_programme)
                     parent_to_children[parent] = _list
                     # parent_to_children[parent] = [child_programme]
@@ -483,45 +459,45 @@
                 # child_to_parents[child_programme] = [parent]
                 if child_programme not in node_layers or node_layers[child_programme] < node_layers[parent]:
                     node_layers[child_programme] = node_layers[parent]
                 elif node_layers[child_programme] > node_layers[parent]:  # cross layer node
                     grand_parents = get_all_parent(child_to_parents, [parent], max_level)
                     for grand_parent in grand_parents:
                         if node_layers[grand_parent] < node_layers[child_programme]:
-                            node_cross_layers[grand_parent] = np_oasis_int(1)
+                            node_cross_layers[grand_parent] = nb_oasis_int(1)
                             node_layers[parent] = node_layers[child_programme]
 
     # compute number of steps (steps), max size of each level node_level_start, max size of node to compute (compute_len)
-    node_level_start = np.zeros(level_node_len.shape[0] + 1, np_oasis_int)
+    node_level_start = np.zeros(level_node_len.shape[0] + 1, oasis_int)
     for i in range(start_level, level_node_len.shape[0]):
         node_level_start[i + 1] = node_level_start[i] + level_node_len[i]
     steps = max_level + (1 - start_level)
     compute_len = node_level_start[-1] + steps + level_node_len[-1] + 1
 
     output_array_size = 0
     for node, layer_size in node_layers.items():
         if node[0] == out_level:
             output_array_size += layer_size
 
     nodes_array = np.empty(node_level_start[-1] + 1, dtype=nodes_array_dtype)
-    node_parents_array = np.empty(parents_len, dtype=np_oasis_int)
+    node_parents_array = np.empty(parents_len, dtype=oasis_int)
     node_profiles_array = np.zeros(fm_policytc.shape[0] + 1, dtype=profile_index_dtype)
-    output_array = np.zeros(output_array_size, dtype=np_oasis_int)
+    output_array = np.zeros(output_array_size, dtype=oasis_int)
 
     node_i = 1
     children_i = 1
     parents_i = 0
     profile_i = 1
     loss_i = 0
     extra_i = 0
     output_i = 0
 
     for level in range(start_level, max_level + 1):
         for agg_id in range(1, level_node_len[level] + 1):
-            node_programme = (np_oasis_int(level), np_oasis_int(agg_id))
+            node_programme = (nb_oasis_int(level), nb_oasis_int(agg_id))
             node = nodes_array[node_i]
             node['node_id'] = node_i
             node_i += 1
             node['level_id'] = level
             node['agg_id'] = agg_id
 
             # layers
@@ -543,15 +519,15 @@
 
             # parent
             if node_programme in child_to_parents:
                 parents = child_to_parents[node_programme]
                 node['parent_len'] = len(parents)
                 node['parent'] = parents_i
                 for parent in parents:
-                    node_parents_array[parents_i], parents_i = node_level_start[parent[0]] + parent[1], np_oasis_int(parents_i + 1)
+                    node_parents_array[parents_i], parents_i = node_level_start[parent[0]] + parent[1], nb_oasis_int(parents_i + 1)
             else:
                 node['parent_len'] = 0
 
             # profiles
             if node_programme in programme_node_to_layers:
                 profiles = programme_node_to_layers[node_programme]
                 if node_programme in node_cross_layers:
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/manager.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import tempfile
-import sys
 import logging
 import numpy as np
 from contextlib import ExitStack
 
 from .financial_structure import create_financial_structure, load_financial_structure
-from .stream_sparse import read_stream_header, EventWriterSparse, read_streams_sparse, EventWriterOrderedOutputSparse
+from .stream_sparse import FMReader, EventWriterSparse, EventWriterOrderedOutputSparse
 from .compute_sparse import compute_event as compute_event_sparse
 from .compute_sparse import init_variable as init_variable_sparse
 from .compute_sparse import reset_variable as reset_variable_sparse
 from .compute_sparse import load_net_value
 from oasislmf.pytools.utils import redirect_logging
+from oasislmf.pytools.common.event_stream import init_streams_in, GUL_STREAM_ID, FM_STREAM_ID, LOSS_STREAM_ID
 
 
 logger = logging.getLogger(__name__)
 
 
 def run(create_financial_structure_files, **kwargs):
     if create_financial_structure_files:
@@ -29,47 +29,40 @@
         allocation_rule = 2
     elif allocation_rule == 0 and net_loss is not None:
         raise NotImplementedError("net loss option is not implemented for alloc rule 0")
 
     if files_out is not None:
         files_out = files_out[0]
 
-    if files_in is None:
-        streams_in = [sys.stdin.buffer]
-    else:
-        streams_in = [open(file_in, 'rb') for file_in in files_in]
+    with ExitStack() as stack:
+        streams_in, (stream_source_type, stream_agg_type, max_sidx_val) = init_streams_in(files_in, stack)
 
-    try:
-        for stream_in in streams_in:
-            stream_type, max_sidx_val = read_stream_header(stream_in)
+        if stream_source_type not in [GUL_STREAM_ID, FM_STREAM_ID, LOSS_STREAM_ID]:
+            raise Exception(f'unsupported stream_type {stream_source_type} (most probable cause is that the up stream data are incorrect)')
 
         if storage_method == "sparse":
-            run_synchronous_sparse(max_sidx_val, allocation_rule, streams_in=streams_in, files_out=files_out, net_loss=net_loss, **kwargs)
+            run_synchronous_sparse(max_sidx_val, allocation_rule, streams_in=streams_in, files_out=files_out, net_loss=net_loss, stack=stack,
+                                   **kwargs)
         else:
             raise ValueError(f"storage_method {storage_method} is not supported for this version")
 
-    finally:
-        if files_in is not None:
-            for stream_in in streams_in:
-                stream_in.close()
-
 
-def run_synchronous_sparse(max_sidx_val, allocation_rule, static_path, streams_in, files_out, low_memory, net_loss, sort_output, **kwargs):
+def run_synchronous_sparse(max_sidx_val, allocation_rule, static_path, streams_in, files_out, low_memory, net_loss, sort_output, stack, **kwargs):
     compute_info, nodes_array, node_parents_array, node_profiles_array, output_array, fm_profile = load_financial_structure(
         allocation_rule, static_path)
 
     compute_info = compute_info[0]
     stepped = True if compute_info['stepped'] else None  # https://github.com/numba/numba/issues/4108
 
     if sort_output:
         event_writer_cls = EventWriterOrderedOutputSparse
     else:
         event_writer_cls = EventWriterSparse
 
-    with tempfile.TemporaryDirectory() as tempdir, ExitStack() as stack:
+    with tempfile.TemporaryDirectory() as tempdir:
         (max_sidx_val, max_sidx_count, len_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val, pass_through,
          extras_indptr, extras_val, children, computes, item_parent_i, compute_idx) = init_variable_sparse(compute_info, max_sidx_val, tempdir, low_memory)
 
         if allocation_rule == 0:
             pass_through_out = np.zeros_like(pass_through)
         else:
             pass_through_out = pass_through
@@ -128,17 +121,18 @@
                     net_loss, nodes_array, output_array, sidx_indexes,
                     sidx_indptr, sidx_val, loss_indptr, loss_val,
                     pass_through_out, max_sidx_val, computes
                 )
             )
             keep_input_loss = True
 
-        for i, event_id in enumerate(read_streams_sparse(
-                streams_in, nodes_array, sidx_indexes, sidx_indptr, sidx_val,
-                loss_indptr, loss_val, pass_through, len_array, computes, compute_idx)):
+        fm_reader = FMReader(nodes_array, sidx_indexes, sidx_indptr, sidx_val,
+                             loss_indptr, loss_val, pass_through, len_array, computes, compute_idx)
+
+        for i, event_id in enumerate(fm_reader.read_streams(streams_in)):
             try:
                 compute_event_sparse(
                     compute_info,
                     keep_input_loss,
                     nodes_array,
                     node_parents_array,
                     node_profiles_array,
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/policy.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/policy.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/policy_extras.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/policy_extras.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fm/stream_sparse.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/stream_sparse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 # sparse array inspired from https://github.com/scipy/scipy/blob/master/scipy/sparse/sparsetools/csr.h
 
 import sys
 import numpy as np
-from numba import jit
-import selectors
-from select import select
+import numba as nb
 import logging
 
+from oasislmf.pytools.common.event_stream import (stream_info_to_bytes, LOSS_STREAM_ID, ITEM_STREAM, PIPE_CAPACITY, EventReader,
+                                                  MAX_LOSS_IDX, CHANCE_OF_LOSS_IDX, TIV_IDX, MEAN_IDX,
+                                                  mv_read, mv_write_item_header, mv_write_sidx_loss, mv_write_delimiter, write_mv_to_stream)
+from oasislmf.pytools.common.data import oasis_int, oasis_int_size, oasis_float, oasis_float_size
+
 logger = logging.getLogger(__name__)
 
 
 remove_empty = False
 
-fm_header = np.int32(1 | 2 << 24).tobytes()
-buff_size = 65536
-event_agg_dtype = np.dtype([('event_id', 'i4'), ('agg_id', 'i4')])
-sidx_loss_dtype = np.dtype([('sidx', 'i4'), ('loss', 'f4')])
-number_size = 8
-nb_number = buff_size // number_size
+
+# buff_size = 65536
+# event_agg_dtype = np.dtype([('event_id', 'i4'), ('agg_id', 'i4')])
+# sidx_loss_dtype = np.dtype([('sidx', 'i4'), ('loss', 'f4')])
+# number_size = 8
+# nb_number = buff_size // number_size
+
+SPECIAL_SIDX_COUNT = 6  # 0 is included as a special sidx
+ITEM_HEADER_SIZE = 2 * oasis_int_size + SPECIAL_SIDX_COUNT * (oasis_int_size + oasis_float_size)
+SIDX_LOSS_WRITE_SIZE = oasis_int_size + oasis_float_size
 
 
-@jit(cache=True, nopython=True)
+@nb.jit(cache=True, nopython=True)
 def reset_empty_items(compute_idx, sidx_indptr, sidx_val, loss_val, computes):
     if remove_empty:
         if sidx_indptr[compute_idx['next_compute_i']] == sidx_indptr[compute_idx['next_compute_i'] - 1]:
 
             computes[compute_idx['next_compute_i']] = 0
             compute_idx['next_compute_i'] -= 1
     else:
         if sidx_indptr[compute_idx['next_compute_i']] == sidx_indptr[compute_idx['next_compute_i'] - 1]:
             sidx_val[sidx_indptr[compute_idx['next_compute_i']]] = -3
             loss_val[sidx_indptr[compute_idx['next_compute_i']]] = 0
             sidx_indptr[compute_idx['next_compute_i']] += 1
 
 
-@jit(cache=True, nopython=True)
+@nb.jit(cache=True, nopython=True)
 def add_new_loss(sidx, loss, compute_i, sidx_indptr, sidx_val, loss_val):
     if ((sidx_indptr[compute_i - 1] == sidx_indptr[compute_i])
             or (sidx_val[sidx_indptr[compute_i] - 1] < sidx)):
         insert_i = sidx_indptr[compute_i]
     else:
         insert_i = np.searchsorted(sidx_val[sidx_indptr[compute_i - 1]: sidx_indptr[compute_i]], sidx) + sidx_indptr[compute_i - 1]
         if sidx_val[insert_i] == sidx:
@@ -46,203 +53,116 @@
         sidx_val[insert_i + 1: sidx_indptr[compute_i] + 1] = sidx_val[insert_i: sidx_indptr[compute_i]]
         loss_val[insert_i + 1: sidx_indptr[compute_i] + 1] = loss_val[insert_i: sidx_indptr[compute_i]]
     sidx_val[insert_i] = sidx
     loss_val[insert_i] = loss
     sidx_indptr[compute_i] += 1
 
 
-def read_stream_header(stream_obj):
-    stream_type = stream_obj.read(4)
-    len_sample = np.frombuffer(stream_obj.read(4), dtype=np.int32)[0]
-    return stream_type, len_sample
-
-
-def register_streams_in(selector_class, streams_in):
-    """
-    Data from input process is generally sent by event block, meaning once a stream receive data, the complete event is
-    going to be sent in a short amount of time.
-    Therefore, we can focus on each stream one by one using their specific selector 'stream_selector'.
-
-    """
-    main_selector = selector_class()
-    stream_data = []
-    for stream_in in streams_in:
-        mv = memoryview(bytearray(buff_size))
-
-        event_agg = np.ndarray(nb_number, buffer=mv, dtype=event_agg_dtype)
-        sidx_loss = np.ndarray(nb_number, buffer=mv, dtype=sidx_loss_dtype)
-
-        stream_selector = selector_class()
-        stream_selector.register(stream_in, selectors.EVENT_READ)
-        data = {'mv': mv,
-                'event_agg': event_agg,
-                'sidx_loss': sidx_loss,
-                'cursor': 0,
-                'valid_buf': 0,
-                'stream_selector': stream_selector
-                }
-        stream_data.append(data)
-        main_selector.register(stream_in, selectors.EVENT_READ, data)
-    return main_selector, stream_data
-
-
-@jit(cache=True, nopython=True)
-def stream_to_loss_sparse(event_agg, sidx_loss, valid_buf, cursor, event_id, agg_id, nodes_array,
-                          sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val, pass_through,
-                          computes, compute_idx):
-    """
-    we use a slithly modified version of the CSR sparse matrix where
-    the column indices for row i are stored in indices[indptr[i]:indptr[i+1]]
-    and their corresponding values are stored in data[indptr[i]:indptr[i+1]].
+def event_log_msg(event_id, sidx_indptr, len_array, node_count):
+    return f"event_id: {event_id}, node_count: {node_count}, sparsity: {100 * sidx_indptr[node_count] / node_count / len_array}"
 
-    nodes_array: array containing all the static information on the nodes
-    loss_indptr: array containing the indexes of the beginning and end of samples of an item
-    loss_sidx: array containing the sidx of the samples
-    loss_val: array containing the loss of the samples
-    # """
-    # sidx_indexes = financial_structure.sidx_indexes
-    # sidx_indptr = financial_structure.sidx_indptr
-    # sidx_val = financial_structure.sidx_val
-    # loss_indptr = financial_structure.loss_indptr
-    # loss_val = financial_structure.loss_val
 
-    valid_len = valid_buf // number_size
+@nb.njit(cache=True)
+def read_buffer(byte_mv, cursor, valid_buff, event_id, item_id,
+                nodes_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val, pass_through,
+                computes, compute_idx
+                ):
     last_event_id = event_id
-
-    while cursor < valid_len:
-        if agg_id:  # we set agg_id to 0 if we expect a new set of event and agg
-            sidx, loss = sidx_loss[cursor]['sidx'], sidx_loss[cursor]['loss']
-            loss = 0 if np.isnan(loss) else loss
-            cursor += 1
+    while True:
+        if item_id:
+            if valid_buff - cursor < (oasis_int_size + oasis_float_size):
+                break
+            sidx, cursor = mv_read(byte_mv, cursor, oasis_int, oasis_int_size)
             if sidx:
-                if loss != 0 and not np.isnan(loss):
+                loss, cursor = mv_read(byte_mv, cursor, oasis_float, oasis_float_size)
+                loss = 0 if np.isnan(loss) else loss
+
+                ###### do loss read ######
+                if loss != 0:
                     if sidx == -2:  # standard deviation
                         pass
                     elif sidx == -4:  # chance of loss
                         pass_through[compute_idx['next_compute_i']] = loss
                     else:
                         add_new_loss(sidx, loss, compute_idx['next_compute_i'], sidx_indptr, sidx_val, loss_val)
+                ##########
             else:
+                ##### do item exit ####
                 reset_empty_items(compute_idx, sidx_indptr, sidx_val, loss_val, computes)
-                agg_id = 0
-
+                ##########
+                cursor += oasis_float_size
+                item_id = 0
         else:
-            event_id, agg_id = event_agg[cursor]['event_id'], event_agg[cursor]['agg_id']
-            cursor += 1
-
+            if valid_buff - cursor < 2 * oasis_int_size:
+                break
+            event_id, cursor = mv_read(byte_mv, cursor, oasis_int, oasis_int_size)
             if event_id != last_event_id:
-                if last_event_id:
-                    return cursor - 1, last_event_id, 0, 1
-                else:
+                if last_event_id:  # we have a new event we return the one we just finished
+                    return cursor - oasis_int_size, last_event_id, 0, 1
+                else:  # first pass we store the event we are reading
                     last_event_id = event_id
-            node = nodes_array[agg_id]
+            item_id, cursor = mv_read(byte_mv, cursor, oasis_int, oasis_int_size)
+
+            ##### do new item setup #####
+            node = nodes_array[item_id]
 
             sidx_indexes[node['node_id']] = compute_idx['next_compute_i']
             loss_indptr[node['loss']: node['loss'] + node['layer_len']] = sidx_indptr[compute_idx['next_compute_i']]
             sidx_indptr[compute_idx['next_compute_i'] + 1] = sidx_indptr[compute_idx['next_compute_i']]
-            computes[compute_idx['next_compute_i']] = agg_id
+            computes[compute_idx['next_compute_i']] = item_id
             compute_idx['next_compute_i'] += 1
+            ##########
+    return cursor, event_id, item_id, 0
 
-    return cursor, event_id, agg_id, 0
-
-
-def read_event_sparse(stream, nodes_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val, pass_through,
-                      computes, compute_idx, main_selector, stream_selector, mv, event_agg, sidx_loss, cursor, valid_buf):
-    event_id = 0
-    agg_id = 0
-
-    while True:
-        if valid_buf < buff_size:
-            len_read = stream.readinto1(mv[valid_buf:])
-            valid_buf += len_read
-
-            if len_read == 0:
-                stream_selector.close()
-                main_selector.unregister(stream)
-                if event_id:
-                    reset_empty_items(compute_idx, sidx_indptr, sidx_val, loss_val, computes)
-                    return event_id, cursor, valid_buf
-
-                break
-
-        cursor, event_id, agg_id, yield_event = stream_to_loss_sparse(
-            event_agg, sidx_loss, valid_buf, cursor,
-            event_id, agg_id, nodes_array,
-            sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val,
-            pass_through, computes, compute_idx)
-
-        if yield_event:
-            if number_size * cursor == valid_buf:
-                valid_buf = 0
-            return event_id, cursor, valid_buf
-        else:
-            cursor_buf = number_size * cursor
-            mv[:valid_buf - cursor_buf] = mv[cursor_buf: valid_buf]
-            valid_buf -= cursor_buf
-            cursor = 0
-            stream_selector.select()
 
+class FMReader(EventReader):
+    """
+    when reading the stream we store relenvant value into a slithly modified version of the CSR sparse matrix where
+    the column indices for row i are stored in indices[indptr[i]:indptr[i+1]]
+    and their corresponding values are stored in data[indptr[i]:indptr[i+1]].
 
-def event_log_msg(event_id, sidx_indptr, len_array, node_count):
-    return f"event_id: {event_id}, node_count: {node_count}, sparsity: {100 * sidx_indptr[node_count] / node_count / len_array}"
+    nodes_array: array containing all the static information on the nodes
+    loss_indptr: array containing the indexes of the beginning and end of samples of an item
+    loss_sidx: array containing the sidx of the samples
+    loss_val: array containing the loss of the samples
+    """
 
+    def __init__(self, nodes_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val, pass_through,
+                 len_array, computes, compute_idx):
+        self.nodes_array = nodes_array
+        self.sidx_indexes = sidx_indexes
+        self.sidx_indptr = sidx_indptr
+        self.sidx_val = sidx_val
+        self.loss_indptr = loss_indptr
+        self.loss_val = loss_val
+        self.pass_through = pass_through
+        self.len_array = len_array
+        self.computes = computes
+        self.compute_idx = compute_idx
+        self.logger = logger
 
-def read_streams_sparse(streams_in, nodes_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val, pass_through,
-                        len_array, computes, compute_idx):
-    try:
-        main_selector, stream_data = register_streams_in(selectors.DefaultSelector, streams_in)
-        logger.debug("Streams read with DefaultSelector")
-    except PermissionError:  # Fall back option if stream_in contain regular files
-        main_selector, stream_data = register_streams_in(selectors.SelectSelector, streams_in)
-        logger.debug("Streams read with SelectSelector")
-    try:
-        while main_selector.get_map():
-            for sKey, _ in main_selector.select():
-                event = read_event_sparse(sKey.fileobj, nodes_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr,
-                                          loss_val, pass_through, computes, compute_idx, main_selector, **sKey.data)
-
-                if event:
-                    event_id, cursor, valid_buf = event
-                    sKey.data['cursor'] = cursor
-                    sKey.data['valid_buf'] = valid_buf
-                    logger.debug(event_log_msg(event_id, sidx_indptr, len_array, compute_idx['next_compute_i']))
-                    yield event_id
-
-        # Stream is read, we need to check if there is remaining event to be parsed
-        for data in stream_data:
-            if data['cursor'] < data['valid_buf']:
-                event_agg = data['event_agg']
-                sidx_loss = data['sidx_loss']
-                cursor = data['cursor']
-                valid_buf = data['valid_buf']
-                yield_event = True
-                while yield_event:
-                    cursor, event_id, agg_id, yield_event = stream_to_loss_sparse(
-                        event_agg,
-                        sidx_loss,
-                        valid_buf,
-                        cursor,
-                        0, 0,
-                        nodes_array,
-                        sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val,
-                        pass_through, computes, compute_idx)
-
-                    if event_id:
-                        reset_empty_items(compute_idx, sidx_indptr, sidx_val, loss_val, computes)
-                        logger.debug(event_log_msg(event_id, sidx_indptr, len_array, compute_idx['next_compute_i']))
-                        yield event_id
+    def read_buffer(self, byte_mv, cursor, valid_buff, event_id, item_id,):
+        return read_buffer(
+            byte_mv, cursor, valid_buff, event_id, item_id,
+            self.nodes_array, self.sidx_indexes, self.sidx_indptr,
+            self.sidx_val, self.loss_indptr, self.loss_val, self.pass_through,
+            self.computes, self.compute_idx
+        )
+
+    def item_exit(self):
+        reset_empty_items(self.compute_idx, self.sidx_indptr, self.sidx_val, self.loss_val, self.computes)
 
-    finally:
-        main_selector.close()
+    def event_read_log(self, event_id):
+        logger.debug(event_log_msg(event_id, self.sidx_indptr, self.len_array, self.compute_idx['next_compute_i']))
 
 
-@jit(cache=True, nopython=True)
-def load_event(event_agg_view, sidx_loss_view, event_id, nodes_array,
+@nb.jit(cache=True, nopython=True)
+def load_event(byte_mv, event_id, nodes_array,
                sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val, pass_through,
-               computes, compute_idx, output_array, i_layer, i_index, nb_values):
+               computes, compute_idx, output_array, i_layer, i_index):
     cursor = 0
     node_id = computes[compute_idx['level_start_compute_i']]
 
     while node_id:
         node = nodes_array[node_id]
         node_sidx_start = sidx_indptr[sidx_indexes[node['node_id']]]
         node_sidx_end = sidx_indptr[sidx_indexes[node['node_id']] + 1]
@@ -250,75 +170,67 @@
         if node_id < pass_through.shape[0]:
             pass_through_loss = pass_through[node_id]
         else:
             pass_through_loss = 0
         for layer in range(i_layer, node['layer_len']):
             output_id = output_array[node['output_ids'] + layer]
             node_loss_start = loss_indptr[node['loss'] + layer]
+
             # print('output_id', output_id)
             # print('    ', sidx_val[node_sidx_start: node_sidx_end])
             # print('    ', loss_val[node_loss_start: node_loss_start + node_val_len])
             if output_id and node_val_len:  # if output is not in xref output_id is 0
                 if i_index == -1:
-                    if nb_values - cursor < 5:  # header + -5, -3, -1 sample
-                        return cursor * number_size, node_id, layer, i_index
-                    else:
-                        # write the header
-                        event_agg_view[cursor]['event_id'], event_agg_view[cursor]['agg_id'] = event_id, output_id
+                    if cursor < PIPE_CAPACITY - ITEM_HEADER_SIZE:  # header + -5, -3, -1 sample
+                        cursor = mv_write_item_header(byte_mv, cursor, event_id, output_id)
                         i_index += 1
-                        cursor += 1
 
-                        if sidx_val[node_sidx_start + i_index] == -5:
-                            sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = -5, loss_val[node_loss_start + i_index]
+                        if sidx_val[node_sidx_start + i_index] == MAX_LOSS_IDX:
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, MAX_LOSS_IDX, loss_val[node_loss_start + i_index])
                             i_index += 1
                         else:
-                            sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = -5, 0
-                        cursor += 1
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, MAX_LOSS_IDX, 0)
 
-                        # write -4 sidx
+                        # write CHANCE_OF_LOSS_IDX == -4 sidx
                         if pass_through_loss:
-                            sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = -4, pass_through_loss
-                            cursor += 1
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, CHANCE_OF_LOSS_IDX, pass_through_loss)
 
-                        # write -3 sidx
-                        if sidx_val[node_sidx_start + i_index] == -3:
-                            sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = -3, loss_val[node_loss_start + i_index]
+                        # write TIV_IDX == -3 sidx
+                        if sidx_val[node_sidx_start + i_index] == TIV_IDX:
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, TIV_IDX, loss_val[node_loss_start + i_index])
                             i_index += 1
                         else:
-                            sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = -3, 0
-                        cursor += 1
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, TIV_IDX, 0)
 
-                        # write -1 sidx
-                        if sidx_val[node_sidx_start + i_index] == -1 and i_index < node_val_len:
-                            sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = -1, loss_val[node_loss_start + i_index]
+                        # write MEAN_IDX == -1 sidx
+                        if sidx_val[node_sidx_start + i_index] == MEAN_IDX and i_index < node_val_len:
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, MEAN_IDX, loss_val[node_loss_start + i_index])
                             i_index += 1
                         else:
-                            sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = -1, 0
-                        cursor += 1
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, MEAN_IDX, 0)
+                    else:
+                        return cursor, node_id, layer, i_index
 
-                while cursor < nb_values:
+                while cursor < PIPE_CAPACITY - SIDX_LOSS_WRITE_SIZE:
                     if i_index == node_val_len:
-                        sidx_loss_view[cursor]['sidx'], sidx_loss_view[cursor]['loss'] = 0, 0
-                        cursor += 1
+                        cursor = mv_write_delimiter(byte_mv, cursor)
                         i_index = -1
                         i_layer = 0
                         break
                     else:
                         if loss_val[node_loss_start + i_index]:
-                            sidx_loss_view[cursor]['sidx'] = sidx_val[node_sidx_start + i_index]
-                            sidx_loss_view[cursor]['loss'] = loss_val[node_loss_start + i_index]
-                            cursor += 1
+                            cursor = mv_write_sidx_loss(byte_mv, cursor, sidx_val[node_sidx_start + i_index], loss_val[node_loss_start + i_index])
                         i_index += 1
 
                 else:
-                    return cursor * number_size, node_id, layer, i_index
+                    return cursor, node_id, layer, i_index
         compute_idx['level_start_compute_i'] += 1
         node_id = computes[compute_idx['level_start_compute_i']]
 
-    return cursor * number_size, node_id, 0, i_index
+    return cursor, node_id, 0, i_index
 
 
 class EventWriterSparse:
     def __init__(self, files_out, nodes_array, output_array, sidx_indexes, sidx_indptr, sidx_val, loss_indptr, loss_val,
                  pass_through, len_sample, computes):
         self.files_out = files_out
         self.nodes_array = nodes_array
@@ -328,59 +240,51 @@
         self.loss_indptr = loss_indptr
         self.loss_val = loss_val
         self.pass_through = pass_through
         self.len_sample = len_sample
         self.computes = computes
         self.output_array = output_array
 
-        self.mv = memoryview(bytearray(nb_number * number_size))
-
-        self.event_agg = np.ndarray(nb_number, buffer=self.mv, dtype=event_agg_dtype)
-        self.sidx_loss = np.ndarray(nb_number, buffer=self.mv, dtype=sidx_loss_dtype)
+        self.byte_mv = np.frombuffer(buffer=memoryview(bytearray(PIPE_CAPACITY)), dtype='b')
 
     def __enter__(self):
         if self.files_out is None:
             self.stream_out = sys.stdout.buffer
         else:
             self.stream_out = open(self.files_out, 'wb')
         # prepare output buffer
-        self.stream_out.write(fm_header)
+        self.stream_out.write(stream_info_to_bytes(LOSS_STREAM_ID, ITEM_STREAM))
         self.stream_out.write(np.int32(self.len_sample).tobytes())
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.files_out:
             self.stream_out.close()
 
     def write(self, event_id, compute_idx):
         i_index = -1
         i_layer = 0
         node_id = 1
-        stream_out = [self.stream_out]
         while node_id:
             cursor, node_id, i_layer, i_index = load_event(
-                self.event_agg,
-                self.sidx_loss,
+                self.byte_mv,
                 event_id,
                 self.nodes_array,
                 self.sidx_indexes, self.sidx_indptr, self.sidx_val, self.loss_indptr, self.loss_val,
                 self.pass_through,
                 self.computes,
                 compute_idx,
                 self.output_array,
                 i_layer,
-                i_index, nb_number)
+                i_index)
 
-            _, writable, exceptional = select([], stream_out, stream_out)
-            if exceptional:
-                raise IOError(f'error with input stream, {exceptional}')
-            writable[0].write(self.mv[:cursor])
+            write_mv_to_stream(self.stream_out, self.byte_mv, cursor)
 
 
-@jit(cache=True, nopython=True)
+@nb.jit(cache=True, nopython=True)
 def get_compute_end(computes, compute_idx):
     compute_start = compute_end = compute_idx['level_start_compute_i']
     while computes[compute_end]:
         compute_end += 1
     return compute_start, compute_end
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/fmpy.py` & `oasislmf-2.3.4/oasislmf/pytools/fm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-from .fm import manager, logger
+from . import manager, logger
 
 import argparse
 import logging
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-a', '--allocation-rule', help='back-allocation rule', default=0, type=int)
 parser.add_argument('-n', '--net-loss', help="if present but empty, write the net instead of the gross in -o output, "
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/footprintconv.py` & `oasislmf-2.3.4/oasislmf/pytools/footprintconv.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/getmodel/common.py` & `oasislmf-2.3.4/oasislmf/pytools/getmodel/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This file defines the data types that are loaded from the data files.
 """
 import numba as nb
 import numpy as np
 
-from oasislmf.pytools.common import areaperil_int, oasis_float
+from oasislmf.pytools.common.data import areaperil_int, oasis_float
 
 # Footprint file formats in order of priority
 fp_format_priorities = ['parquet', 'binZ', 'bin', 'csv']
 
 # filenames
 footprint_filename = 'footprint.bin'
 footprint_index_filename = 'footprint.idx'
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/getmodel/footprint.py` & `oasislmf-2.3.4/oasislmf/pytools/getmodel/footprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,29 @@
         self.storage = storage
         self.stack = ExitStack()
         self.df_engine = df_engine
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.stack.__exit__(exc_type, exc_value, exc_traceback)
 
+    @staticmethod
+    def get_footprint_fmt_priorities():
+        """
+        Get list of footprint file format classes in order of priority.
+
+        Returns: (list) footprint file format classes
+        """
+        format_to_class = {
+            'parquet': FootprintParquet, 'csv': FootprintCsv,
+            'binZ': FootprintBinZ, 'bin': FootprintBin,
+        }
+        priorities = [format_to_class[fmt] for fmt in fp_format_priorities if fmt in format_to_class]
+
+        return priorities
+
     @classmethod
     def load(
         cls,
         storage: BaseStorage,
         ignore_file_type=set(),
         df_engine="oasis_data_manager.df_reader.reader.OasisPandasReader",
     ):
@@ -94,21 +109,15 @@
             json
             z
             bin
             idx
 
         Returns: (Union[FootprintBinZ, FootprintBin, FootprintCsv]) the loaded class
         """
-        format_to_class = {
-            'parquet': FootprintParquet, 'csv': FootprintCsv,
-            'binZ': FootprintBinZ, 'bin': FootprintBin,
-        }
-        priorities = [format_to_class[fmt] for fmt in fp_format_priorities if fmt in format_to_class]
-
-        for footprint_class in priorities:
+        for footprint_class in cls.get_footprint_fmt_priorities():
             for filename in footprint_class.footprint_filenames:
                 if (not storage.exists(filename)
                         or filename.rsplit('.', 1)[-1] in ignore_file_type):
                     valid = False
                     break
             else:
                 valid = True
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/getmodel/manager.py` & `oasislmf-2.3.4/oasislmf/pytools/getmodel/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from numba import int32 as nb_int32, float64 as nb_float64
 from numba.typed import Dict
 
 from oasis_data_manager.df_reader.config import get_df_reader, clean_config, InputReaderConfig
 from oasis_data_manager.filestore.backends.base import BaseStorage
 from oasis_data_manager.filestore.config import get_storage_from_config_path
-from oasislmf.pytools.common import PIPE_CAPACITY
+from oasislmf.pytools.common.event_stream import PIPE_CAPACITY
 from oasislmf.utils.data import validate_vulnerability_replacements
 from oasislmf.pytools.data_layer.footprint_layer import FootprintLayerClient
 from oasislmf.pytools.getmodel.common import (Index_type, Keys, areaperil_int,
                                               oasis_float)
 from oasislmf.pytools.getmodel.footprint import Footprint
 from oasislmf.pytools.utils import redirect_logging
 from ods_tools.oed import AnalysisSettingSchema
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/getmodel/vulnerability.py` & `oasislmf-2.3.4/oasislmf/pytools/getmodel/vulnerability.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import List, Tuple
 
 import numba as nb
 import numpy as np
 import pyarrow as pa
 import pyarrow.parquet as pq
 
-from oasislmf.pytools.common import oasis_float
+from oasislmf.pytools.common.data import oasis_float
 
 from .common import Vulnerability
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gul/common.py` & `oasislmf-2.3.4/oasislmf/pytools/gulmc/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,50 @@
-"""
-This file defines the data types that are loaded from the data files.
-
-"""
 import numba as nb
 import numpy as np
 
-from oasislmf.pytools.common import areaperil_int, oasis_float
+from oasislmf.pytools.common.data import areaperil_int, oasis_float
 
 # gul stream type
 # probably need to set this dynamically depending on the stream type
 gul_header = np.int32(1 | 2 << 24).tobytes()
 
+Item = nb.from_dtype(np.dtype([('item_id', np.int32),
+                               ('coverage_id', np.int32),
+                               ('areaperil_id', areaperil_int),
+                               ('vulnerability_id', np.int32),
+                               ('group_id', np.int32)
+                               ]))
+
 items_data_type = nb.from_dtype(np.dtype([('item_id', np.int32),
                                           ('damagecdf_i', np.int32),
                                           ('rng_index', np.int32)
                                           ]))
 
 items_MC_data_type = nb.from_dtype(np.dtype([('item_id', np.int32),
-                                             ('areaperil_id', areaperil_int),
-                                             ('vulnerability_id', np.int32),
+                                             ('item_idx', np.int32),
                                              ('hazcdf_i', np.int32),
                                              ('rng_index', np.int32),
                                              ('hazard_rng_index', np.int32),
-                                             ('eff_vuln_cdf_i', np.int32),
-                                             ('eff_vuln_cdf_Ndamage_bins', np.int32)
                                              ]))
 
 VulnCdfLookup = nb.from_dtype(np.dtype([('start', np.int32), ('length', np.int32)]))
 
 
 coverage_type = nb.from_dtype(np.dtype([('tiv', np.float64),
                                         ('max_items', np.int32),
                                         ('start_items', np.int32),
                                         ('cur_items', np.int32)
                                         ]))
 
 NP_BASE_ARRAY_SIZE = 8
 
-# negative sidx (definition)
-MEAN_IDX = -1
-STD_DEV_IDX = -2
-TIV_IDX = -3
-CHANCE_OF_LOSS_IDX = -4
-MAX_LOSS_IDX = -5
-
-NUM_IDX = 5
 
 ITEM_MAP_KEY_TYPE = nb.types.Tuple((nb.from_dtype(areaperil_int), nb.types.int32))
-ITEM_MAP_VALUE_TYPE = nb.types.UniTuple(nb.types.int32, 3)
+# ITEM_MAP_VALUE_TYPE = nb.types.UniTuple(nb.types.int32, 1)
+ITEM_MAP_VALUE_TYPE = nb.types.int64
 AREAPERIL_TO_EFF_VULN_KEY_TYPE = nb.types.Tuple((nb.from_dtype(areaperil_int), nb.types.int64))
 AREAPERIL_TO_EFF_VULN_VALUE_TYPE = nb.types.UniTuple(nb.types.int32, 2)
 
 # compute the relative size of oasis_float and areaperil_int vs int32
 oasis_float_to_int32_size = oasis_float.itemsize // np.int32().itemsize
 areaperil_int_to_int32_size = areaperil_int.itemsize // np.int32().itemsize
 
@@ -85,7 +78,15 @@
 
 
 Keys = {'LocID': np.int32,
         'PerilID': 'category',
         'CoverageTypeID': np.int32,
         'AreaPerilID': areaperil_int,
         'VulnerabilityID': np.int32}
+
+
+NormInversionParameters = nb.from_dtype(np.dtype([('x_min', np.float32),
+                                                  ('x_max', np.float32),
+                                                  ('N', np.int32),
+                                                  ('cdf_min', np.float32),
+                                                  ('cdf_max', np.float32),
+                                                  ]))
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gul/core.py` & `oasislmf-2.3.4/oasislmf/pytools/gul/core.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gul/manager.py` & `oasislmf-2.3.4/oasislmf/pytools/gul/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,40 +10,62 @@
 
 import numpy as np
 import pandas as pd
 from numba import njit
 from numba.typed import Dict, List
 
 from oasis_data_manager.filestore.config import get_storage_from_config_path
-from oasislmf.pytools.common import PIPE_CAPACITY
-from oasislmf.pytools.data_layer.oasis_files.correlations import (
-    Correlation, CorrelationsData)
+from oasislmf.pytools.common.event_stream import (PIPE_CAPACITY, mv_write_item_header, mv_write_sidx_loss, mv_write_delimiter,
+                                                  stream_info_to_bytes, LOSS_STREAM_ID, ITEM_STREAM)
+from oasislmf.pytools.data_layer.oasis_files.correlations import Correlation, CorrelationsData
 from oasislmf.pytools.getmodel.common import Keys, oasis_float
 from oasislmf.pytools.getmodel.manager import Item, get_damage_bins
-from oasislmf.pytools.gul.common import (CHANCE_OF_LOSS_IDX, ITEM_MAP_KEY_TYPE,
+from oasislmf.pytools.gul.common import (SPECIAL_SIDX, CHANCE_OF_LOSS_IDX, ITEM_MAP_KEY_TYPE,
                                          ITEM_MAP_VALUE_TYPE, MAX_LOSS_IDX,
                                          MEAN_IDX, NUM_IDX, STD_DEV_IDX,
-                                         TIV_IDX, coverage_type, gul_header,
+                                         TIV_IDX, coverage_type,
                                          gulSampleslevelHeader_size,
                                          gulSampleslevelRec_size)
 from oasislmf.pytools.gul.core import (compute_mean_loss, get_gul, setmaxloss,
                                        split_tiv_classic,
                                        split_tiv_multiplicative)
-from oasislmf.pytools.gul.io import (read_getmodel_stream, write_negative_sidx,
-                                     write_sample_header, write_sample_rec)
+from oasislmf.pytools.gul.io import read_getmodel_stream
 from oasislmf.pytools.gul.random import (compute_norm_cdf_lookup,
                                          compute_norm_inv_cdf_lookup,
                                          generate_correlated_hash_vector,
                                          get_corr_rval, get_random_generator)
 from oasislmf.pytools.gul.utils import append_to_dict_value, binary_search
 from oasislmf.pytools.utils import redirect_logging
 
 logger = logging.getLogger(__name__)
 
 
+@njit(cache=True)
+def adjust_byte_mv_size(byte_mv, max_bytes_per_coverage):
+    """
+    adjust buff size so that the buffer fits the longest coverage
+    Args:
+        byte_mv: numpy byte array
+        max_bytes_per_coverage: max size possible to accommodate all the coverage in byte_mv
+
+    Returns:
+        byte_mv: numpy byte array
+    """
+    #
+    buff_size = byte_mv.shape[0]
+    while buff_size < max_bytes_per_coverage:
+        buff_size *= 2
+
+    if byte_mv.shape[0] < buff_size:
+        # create a new bigger byte_mv
+        byte_mv = np.empty(buff_size, dtype='b')
+
+    return byte_mv
+
+
 def get_coverages(input_path, ignore_file_type=set()):
     """Load the coverages from the coverages file.
 
     Args:
         input_path (str): the path containing the coverage file.
         ignore_file_type (Set[str]): file extension to ignore when loading.
 
@@ -199,25 +221,24 @@
             stream_out = sys.stdout.buffer
         else:
             stream_out = stack.enter_context(open(file_out, 'wb'))
 
         select_stream_list = [stream_out]
 
         # prepare output buffer, write stream header
-        stream_out.write(gul_header)
+        stream_out.write(stream_info_to_bytes(LOSS_STREAM_ID, ITEM_STREAM))
         stream_out.write(np.int32(sample_size).tobytes())
 
         # set the random generator function
         generate_rndm = get_random_generator(random_generator)
 
         if alloc_rule not in [0, 1, 2, 3]:
             raise ValueError(f"Expect alloc_rule to be 0, 1, 2, or 3, got {alloc_rule}")
 
         cursor = 0
-        cursor_bytes = 0
 
         # create the array to store the seeds
         seeds = np.zeros(len(np.unique(items['group_id'])), dtype=Item.dtype['group_id'])
 
         do_correlation = False
         if ignore_correlation:
             logger.info("Correlated random number generation: switched OFF because --ignore-correlation is True.")
@@ -266,17 +287,18 @@
             arr_min, arr_max, arr_N = 0, 0, 0
             arr_min_cdf, arr_max_cdf = 0, 0
             norm_inv_cdf, norm_cdf = np.zeros(1, dtype='float64'), np.zeros(1, dtype='float64')
             z_unif = np.zeros(1, dtype='float64')
 
         # create buffer to be reused to store all losses for one coverage
         losses_buffer = np.zeros((sample_size + NUM_IDX + 1, np.max(coverages[1:]['max_items'])), dtype=oasis_float)
+        byte_mv = np.empty(PIPE_CAPACITY * 2, dtype='b')
 
         # maximum bytes to be written in the output stream for 1 item
-        max_bytes_per_item = (sample_size + NUM_IDX + 1) * gulSampleslevelRec_size + 2 * gulSampleslevelHeader_size
+        max_bytes_per_item = gulSampleslevelHeader_size + (sample_size + NUM_IDX + 1) * gulSampleslevelRec_size
 
         for event_data in read_getmodel_stream(streams_in, item_map, coverages, compute, seeds, valid_area_peril_id):
 
             event_id, compute_i, items_data, recs, rec_idx_ptr, rng_index = event_data
 
             # generation of "base" random values is done as before
             rndms_base = generate_rndm(seeds[:rng_index], sample_size)
@@ -291,51 +313,44 @@
                 # create dummy data structures with proper dtypes to allow correct numba compilation
                 corr_seeds = np.zeros(1, dtype='int64')
                 eps_ij = np.zeros((1, 1), dtype='float64')
 
             last_processed_coverage_ids_idx = 0
 
             # adjust buff size so that the buffer fits the longest coverage
-            buff_size = PIPE_CAPACITY * 2
-            max_bytes_per_coverage = np.max(coverages['cur_items']) * max_bytes_per_item
-            while buff_size < max_bytes_per_coverage:
-                buff_size *= 2
-
-            # define the raw memory view and its int32 view
-            mv_write = memoryview(bytearray(buff_size))
-            int32_mv_write = np.ndarray(buff_size // 4, buffer=mv_write, dtype='i4')
+            byte_mv = adjust_byte_mv_size(byte_mv, np.max(coverages['cur_items']) * max_bytes_per_item)
 
             while last_processed_coverage_ids_idx < compute_i:
-                cursor, cursor_bytes, last_processed_coverage_ids_idx = compute_event_losses(
+                cursor, last_processed_coverage_ids_idx = compute_event_losses(
                     event_id, coverages, compute[:compute_i], items_data,
                     last_processed_coverage_ids_idx, sample_size, recs, rec_idx_ptr,
                     damage_bins, loss_threshold, losses_buffer, alloc_rule, do_correlation, rndms_base, eps_ij, corr_data_by_item_id,
                     arr_min, arr_max, arr_N, norm_inv_cdf, arr_min_cdf, arr_max_cdf, norm_cdf, z_unif, debug,
-                    max_bytes_per_item, buff_size, int32_mv_write, cursor
+                    max_bytes_per_item, byte_mv, cursor
                 )
 
                 # write the losses to the output stream
                 write_start = 0
-                while write_start < cursor_bytes:
+                while write_start < cursor:
                     select([], select_stream_list, select_stream_list)
-                    write_start += stream_out.write(mv_write[write_start:cursor_bytes])
+                    write_start += stream_out.write(byte_mv[write_start:cursor].tobytes())
 
                 cursor = 0
 
             logger.info(f"event {event_id} DONE")
 
     return 0
 
 
 @njit(cache=True, fastmath=True)
 def compute_event_losses(event_id, coverages, coverage_ids, items_data,
                          last_processed_coverage_ids_idx, sample_size, recs, rec_idx_ptr, damage_bins,
                          loss_threshold, losses, alloc_rule, do_correlation, rndms_base, eps_ij, corr_data_by_item_id,
                          arr_min, arr_max, arr_N, norm_inv_cdf, arr_min_cdf, arr_max_cdf, norm_cdf,
-                         z_unif, debug, max_bytes_per_item, buff_size, int32_mv, cursor):
+                         z_unif, debug, max_bytes_per_item, byte_mv, cursor):
     """Compute losses for an event.
 
     Args:
         event_id (int32): event id.
         coverages (numpy.array[oasis_float]): array with the coverage values for each coverage_id.
         coverage_ids (numpy.array[int]): array of unique coverage ids used in this event.
         items_data (numpy.array[items_data_type]): items-related data.
@@ -350,37 +365,35 @@
         alloc_rule (int): back-allocation rule.
         do_correlation (bool): if True, compute correlated random samples.
         rndms (numpy.array[float64]): 2d array of shape (number of seeds, sample_size) storing the random values
           drawn for each seed.
         debug (bool): if True, for each random sample, print to the output stream the random value
           instead of the loss.
         max_bytes_per_item (int): maximum bytes to be written in the output stream for an item.
-        buff_size (int): size in bytes of the output buffer.
-        int32_mv (numpy.ndarray): int32 view of the memoryview where the output is buffered.
+        byte_mv (numpy.array): byte view of where the output is buffered.
         cursor (int): index of int32_mv where to start writing.
 
     Returns:
-        int, int, int: updated value of cursor, updated value of cursor_bytes, last last_processed_coverage_ids_idx
+        int, int: updated value of cursor, last last_processed_coverage_ids_idx
     """
     for coverage_i in range(last_processed_coverage_ids_idx, coverage_ids.shape[0]):
         coverage = coverages[coverage_ids[coverage_i]]
         tiv = coverage['tiv']  # coverages are indexed from 1
         Nitem_ids = coverage['cur_items']
         exposureValue = tiv / Nitem_ids
 
         # estimate max number of bytes needed to output this coverage
         # conservatively assume all random samples are printed (losses>loss_threshold)
         # number of records of type gulSampleslevelRec_size is sample_size + 5 (negative sidx) + 1 (terminator line)
-        cursor_bytes = cursor * int32_mv.itemsize
         est_cursor_bytes = Nitem_ids * max_bytes_per_item
 
         # return before processing this coverage if the number of free bytes left in the buffer
         # is not sufficient to write out the full coverage
-        if cursor_bytes + est_cursor_bytes > buff_size:
-            return cursor, cursor_bytes, last_processed_coverage_ids_idx
+        if cursor + est_cursor_bytes > byte_mv.shape[0]:
+            return cursor, last_processed_coverage_ids_idx
 
         items = items_data[coverage['start_items']: coverage['start_items'] + coverage['cur_items']]
 
         for item_i in range(coverage['cur_items']):
             item = items[item_i]
             damagecdf_i = item['damagecdf_i']
             rng_index = item['rng_index']
@@ -452,36 +465,36 @@
 
                         if gul >= loss_threshold:
                             losses[sample_idx, item_i] = gul
                         else:
                             losses[sample_idx, item_i] = 0
 
         cursor = write_losses(event_id, sample_size, loss_threshold, losses[:, :items.shape[0]], items['item_id'], alloc_rule, tiv,
-                              int32_mv, cursor)
+                              byte_mv, cursor)
 
         # register that another `coverage_id` has been processed
         last_processed_coverage_ids_idx += 1
 
-    return cursor, cursor * int32_mv.itemsize, last_processed_coverage_ids_idx
+    return cursor, last_processed_coverage_ids_idx
 
 
 @njit(cache=True, fastmath=True)
 def write_losses(event_id, sample_size, loss_threshold, losses, item_ids, alloc_rule, tiv,
-                 int32_mv, cursor):
+                 byte_mv, cursor):
     """Write the computed losses.
 
     Args:
         event_id (int32): event id.
         sample_size (int): number of random samples to draw.
         loss_threshold (float): threshold above which losses are printed to the output stream.
         losses (numpy.array[oasis_float]): losses for all item_ids
         item_ids (numpy.array[ITEM_ID_TYPE]): ids of items whose losses are in `losses`.
         alloc_rule (int): back-allocation rule.
         tiv (oasis_float): total insured value.
-        int32_mv (numpy.ndarray): int32 view of the memoryview where the output is buffered.
+        byte_mv (numpy.ndarray): byte view of where the output is buffered.
         cursor (int): index of int32_mv where to start writing.
 
     Returns:
         int: updated values of cursor
     """
     if alloc_rule == 2:
         losses[1:] = setmaxloss(losses[1:])
@@ -500,30 +513,22 @@
             for sample_i in range(1, losses.shape[0]):
                 split_tiv_multiplicative(losses[sample_i], tiv)
 
     # output the losses for all the items
     for item_j in range(item_ids.shape[0]):
 
         # write header
-        cursor = write_sample_header(
-            event_id, item_ids[item_j], int32_mv, cursor)
+        cursor = mv_write_item_header(byte_mv, cursor, event_id, item_ids[item_j])
 
         # write negative sidx
-        cursor = write_negative_sidx(
-            MAX_LOSS_IDX, losses[MAX_LOSS_IDX, item_j],
-            CHANCE_OF_LOSS_IDX, losses[CHANCE_OF_LOSS_IDX, item_j],
-            TIV_IDX, losses[TIV_IDX, item_j],
-            STD_DEV_IDX, losses[STD_DEV_IDX, item_j],
-            MEAN_IDX, losses[MEAN_IDX, item_j],
-            int32_mv, cursor
-        )
+        for sample_idx in SPECIAL_SIDX:
+            cursor = mv_write_sidx_loss(byte_mv, cursor, sample_idx, losses[sample_idx, item_j])
 
         # write the random samples (only those with losses above the threshold)
         for sample_idx in range(1, sample_size + 1):
             if losses[sample_idx, item_j] >= loss_threshold:
-                cursor = write_sample_rec(
-                    sample_idx, losses[sample_idx, item_j], int32_mv, cursor)
+                cursor = mv_write_sidx_loss(byte_mv, cursor, sample_idx, losses[sample_idx, item_j])
 
         # write terminator for the samples for this item
-        cursor = write_sample_rec(0, 0., int32_mv, cursor)
+        cursor = mv_write_delimiter(byte_mv, cursor)
 
     return cursor
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gul/random.py` & `oasislmf-2.3.4/oasislmf/pytools/gul/random.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gul/utils.py` & `oasislmf-2.3.4/oasislmf/pytools/gul/utils.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gulmc/aggregate.py` & `oasislmf-2.3.4/oasislmf/pytools/gulmc/aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from numba import njit
 from numba.typed import Dict, List
 from numba.types import int32 as nb_int32
 from numba.types import uint32 as nb_uint32
 from numba.types import float32 as nb_float32
 
 from oasis_data_manager.filestore.backends.base import BaseStorage
-from oasislmf.pytools.common import areaperil_int
+from oasislmf.pytools.common.data import areaperil_int
 
 logger = logging.getLogger(__name__)
 
 AGG_VULN_WEIGHTS_KEY_TYPE = nb.types.Tuple((nb.from_dtype(areaperil_int), nb.types.int32))
 AGG_VULN_WEIGHTS_VAL_TYPE = nb.types.float32
 
 AggregateVulnerability = nb.from_dtype(np.dtype([('aggregate_vulnerability_id', np.int32),
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gulmc/cli.py` & `oasislmf-2.3.4/oasislmf/pytools/gulmc/cli.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gulmc/items.py` & `oasislmf-2.3.4/oasislmf/pytools/gulmc/items.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 from numba import njit
 from numba.typed import Dict, List
 from numba.types import int32 as nb_int32
 from numba.types import int64 as nb_int64
 
-from oasislmf.pytools.common import nb_areaperil_int
+from oasislmf.pytools.common.data import nb_areaperil_int
 from oasislmf.pytools.getmodel.common import Index_type
 from oasislmf.pytools.gul.utils import append_to_dict_value
 from oasislmf.pytools.gulmc.aggregate import gen_empty_agg_vuln_to_vuln_ids
 from oasislmf.pytools.gulmc.common import (ITEM_MAP_KEY_TYPE,
                                            ITEM_MAP_VALUE_TYPE, Item)
 
 logger = logging.getLogger(__name__)
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gulmc/manager.py` & `oasislmf-2.3.4/oasislmf/pytools/gulmc/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,34 +12,36 @@
 from numba import njit
 from numba.typed import Dict, List
 from numba.types import Tuple as nb_Tuple
 from numba.types import int32 as nb_int32
 from numba.types import int64 as nb_int64
 
 from oasis_data_manager.filestore.config import get_storage_from_config_path
-from oasislmf.pytools.common import PIPE_CAPACITY, nb_areaperil_int, oasis_float
+from oasislmf.pytools.common.data import nb_areaperil_int, oasis_float
+from oasislmf.pytools.common.event_stream import PIPE_CAPACITY
 from oasislmf.pytools.data_layer.footprint_layer import FootprintLayerClient
 from oasislmf.pytools.data_layer.oasis_files.correlations import Correlation, read_correlations
 from oasislmf.pytools.getmodel.footprint import Footprint
 from oasislmf.pytools.getmodel.manager import get_damage_bins, get_vulns, get_vuln_rngadj_dict, convert_vuln_id_to_index
+from oasislmf.pytools.gul.common import MAX_LOSS_IDX, CHANCE_OF_LOSS_IDX, TIV_IDX, STD_DEV_IDX, MEAN_IDX, NUM_IDX
 from oasislmf.pytools.gul.core import compute_mean_loss, get_gul
-from oasislmf.pytools.gul.manager import get_coverages, write_losses
+from oasislmf.pytools.gul.manager import get_coverages, write_losses, adjust_byte_mv_size
 from oasislmf.pytools.gul.random import (compute_norm_cdf_lookup, compute_norm_inv_cdf_lookup,
                                          generate_correlated_hash_vector, generate_hash,
                                          generate_hash_hazard, get_corr_rval, get_random_generator)
 from oasislmf.pytools.gul.utils import binary_search
 from oasislmf.pytools.gulmc.aggregate import (
     map_agg_vuln_ids_to_agg_vuln_idxs,
     map_areaperil_vuln_id_to_weight_to_areaperil_vuln_idx_to_weight,
     process_aggregate_vulnerability, process_vulnerability_weights, read_aggregate_vulnerability,
     read_vulnerability_weights)
 from oasislmf.pytools.gulmc.common import (AREAPERIL_TO_EFF_VULN_KEY_TYPE,
-                                           AREAPERIL_TO_EFF_VULN_VALUE_TYPE, CHANCE_OF_LOSS_IDX,
-                                           MAX_LOSS_IDX, MEAN_IDX, NP_BASE_ARRAY_SIZE, NUM_IDX,
-                                           STD_DEV_IDX, TIV_IDX, Item, Keys,
+                                           AREAPERIL_TO_EFF_VULN_VALUE_TYPE,
+                                           NP_BASE_ARRAY_SIZE,
+                                           Item, Keys,
                                            NormInversionParameters, coverage_type, gul_header,
                                            gulSampleslevelHeader_size, gulSampleslevelRec_size,
                                            haz_cdf_type, items_MC_data_type)
 from oasislmf.pytools.gulmc.items import generate_item_map, process_items, read_items
 from oasislmf.pytools.utils import redirect_logging
 
 logger = logging.getLogger(__name__)
@@ -245,15 +247,14 @@
 
         select_stream_list = [stream_out]
 
         # prepare output stream
         stream_out.write(gul_header)
         stream_out.write(np.int32(sample_size).tobytes())
         cursor = 0
-        cursor_bytes = 0
 
         # set the random generator function
         generate_rndm = get_random_generator(random_generator)
         # create the array to store the seeds
         haz_seeds = np.zeros(len(np.unique(items['hazard_group_id'])), dtype=Correlation.dtype['hazard_group_id'])
         vuln_seeds = np.zeros(len(np.unique(items['group_id'])), dtype=Item.dtype['group_id'])
 
@@ -308,20 +309,21 @@
         if effective_damageability is True:
             logger.info("effective_damageability is True: gulmc will draw the damage samples from the effective damageability distribution.")
         else:
             logger.info("effective_damageability is False: gulmc will perform the full Monte Carlo sampling: "
                         "sample the hazard intensity first, then sample the damage from the corresponding vulnerability function.")
 
         # create buffers to be reused when computing losses
+        byte_mv = np.empty(PIPE_CAPACITY * 2, dtype='b')
         losses = np.zeros((sample_size + NUM_IDX + 1, np.max(coverages[1:]['max_items'])), dtype=oasis_float)
         vuln_cdf_empty = np.zeros(Ndamage_bins_max, dtype=oasis_float)
         weighted_vuln_cdf_empty = np.zeros(Ndamage_bins_max, dtype=oasis_float)
 
         # maximum bytes to be written in the output stream for 1 item
-        max_bytes_per_item = (sample_size + NUM_IDX + 1) * gulSampleslevelRec_size + 2 * gulSampleslevelHeader_size
+        max_bytes_per_item = gulSampleslevelHeader_size + (sample_size + NUM_IDX + 1) * gulSampleslevelRec_size
 
         # define vulnerability cdf cache size
         max_cached_vuln_cdf_size_bytes = max_cached_vuln_cdf_size_MB * 1024 * 1024  # cahce size in bytes
         max_Nnumbers_cached_vuln_cdf = max_cached_vuln_cdf_size_bytes // oasis_float.itemsize  # total numbers that can fit in the cache
         max_Nvulnerability_cached_vuln_cdf = max_Nnumbers_cached_vuln_cdf // Ndamage_bins_max  # max number of vulnerability funcions that can be stored in cache
         # number of vulnerability functions to be cached
         Nvulns_cached = min(Nvulnerability * Nintensity_bins, max_Nvulnerability_cached_vuln_cdf)
@@ -383,81 +385,73 @@
 
                 else:
                     # create dummy data structures with proper dtypes to allow correct numba compilation
                     eps_ij = np.zeros((1, 1), dtype='float64')
 
                 last_processed_coverage_ids_idx = 0
 
-                # adjust buff size so that the buffer fits the longest coverage
-                buff_size = PIPE_CAPACITY
-                max_bytes_per_coverage = np.max(coverages['cur_items']) * max_bytes_per_item
-                while buff_size < max_bytes_per_coverage:
-                    buff_size *= 2
-
-                # define the raw memory view and its int32 view
-                mv_write = memoryview(bytearray(buff_size))
-                int32_mv = np.ndarray(buff_size // 4, buffer=mv_write, dtype='i4')
+                byte_mv = adjust_byte_mv_size(byte_mv, np.max(coverages['cur_items']) * max_bytes_per_item)
 
                 # create vulnerability cdf cache
                 cached_vuln_cdfs = np.zeros((Nvulns_cached, Ndamage_bins_max), dtype=oasis_float)
                 cached_vuln_cdf_lookup, lookup_keys = gen_empty_vuln_cdf_lookup(Nvulns_cached)
                 next_cached_vuln_cdf = 0
 
                 while last_processed_coverage_ids_idx < compute_i:
 
-                    cursor, cursor_bytes, last_processed_coverage_ids_idx, next_cached_vuln_cdf = compute_event_losses(event_id,
-                                                                                                                       coverages,
-                                                                                                                       compute[:compute_i],
-                                                                                                                       items_event_data,
-                                                                                                                       items,
-                                                                                                                       last_processed_coverage_ids_idx,
-                                                                                                                       sample_size,
-                                                                                                                       haz_cdf,
-                                                                                                                       haz_cdf_ptr,
-                                                                                                                       areaperil_to_eff_vuln_cdf,
-                                                                                                                       eff_vuln_cdf,
-                                                                                                                       vuln_array,
-                                                                                                                       damage_bins,
-                                                                                                                       Ndamage_bins_max,
-                                                                                                                       cached_vuln_cdf_lookup,
-                                                                                                                       lookup_keys,
-                                                                                                                       next_cached_vuln_cdf,
-                                                                                                                       cached_vuln_cdfs,
-                                                                                                                       agg_vuln_to_vuln_id,
-                                                                                                                       agg_vuln_to_vuln_idxs,
-                                                                                                                       vuln_dict,
-                                                                                                                       areaperil_vuln_idx_to_weight,
-                                                                                                                       loss_threshold,
-                                                                                                                       losses,
-                                                                                                                       vuln_cdf_empty,
-                                                                                                                       weighted_vuln_cdf_empty,
-                                                                                                                       alloc_rule,
-                                                                                                                       do_correlation,
-                                                                                                                       do_haz_correlation,
-                                                                                                                       haz_rndms_base,
-                                                                                                                       vuln_rndms_base,
-                                                                                                                       vuln_adj_dict,
-                                                                                                                       haz_eps_ij,
-                                                                                                                       eps_ij,
-                                                                                                                       norm_inv_parameters,
-                                                                                                                       norm_inv_cdf,
-                                                                                                                       norm_cdf,
-                                                                                                                       z_unif,
-                                                                                                                       effective_damageability,
-                                                                                                                       debug,
-                                                                                                                       max_bytes_per_item,
-                                                                                                                       buff_size,
-                                                                                                                       int32_mv,
-                                                                                                                       cursor)
+                    cursor, last_processed_coverage_ids_idx, next_cached_vuln_cdf = compute_event_losses(
+                        event_id,
+                        coverages,
+                        compute[:compute_i],
+                        items_event_data,
+                        items,
+                        last_processed_coverage_ids_idx,
+                        sample_size,
+                        haz_cdf,
+                        haz_cdf_ptr,
+                        areaperil_to_eff_vuln_cdf,
+                        eff_vuln_cdf,
+                        vuln_array,
+                        damage_bins,
+                        Ndamage_bins_max,
+                        cached_vuln_cdf_lookup,
+                        lookup_keys,
+                        next_cached_vuln_cdf,
+                        cached_vuln_cdfs,
+                        agg_vuln_to_vuln_id,
+                        agg_vuln_to_vuln_idxs,
+                        vuln_dict,
+                        areaperil_vuln_idx_to_weight,
+                        loss_threshold,
+                        losses,
+                        vuln_cdf_empty,
+                        weighted_vuln_cdf_empty,
+                        alloc_rule,
+                        do_correlation,
+                        do_haz_correlation,
+                        haz_rndms_base,
+                        vuln_rndms_base,
+                        vuln_adj_dict,
+                        haz_eps_ij,
+                        eps_ij,
+                        norm_inv_parameters,
+                        norm_inv_cdf,
+                        norm_cdf,
+                        z_unif,
+                        effective_damageability,
+                        debug,
+                        max_bytes_per_item,
+                        byte_mv,
+                        cursor)
 
                     # write the losses to the output stream
                     write_start = 0
-                    while write_start < cursor_bytes:
+                    while write_start < cursor:
                         select([], select_stream_list, select_stream_list)
-                        write_start += stream_out.write(mv_write[write_start:cursor_bytes])
+                        write_start += stream_out.write(byte_mv[write_start:cursor].tobytes())
 
                     cursor = 0
 
                 logger.info(f"event {event_id} DONE")
 
     return 0
 
@@ -500,16 +494,15 @@
                          norm_inv_parameters,
                          norm_inv_cdf,
                          norm_cdf,
                          z_unif,
                          effective_damageability,
                          debug,
                          max_bytes_per_item,
-                         buff_size,
-                         int32_mv,
+                         byte_mv,
                          cursor):
     """Compute losses for an event.
 
     Args:
         event_id (int32): event id.
         coverages (numpy.array[oasis_float]): array with the coverage values for each coverage_id.
         coverage_ids (numpy.array[int]): array of unique coverage ids used in this event.
@@ -556,40 +549,38 @@
         norm_cdf (np.array[float]): Gaussian cdf.
         z_unif (np.array[float]): buffer to be re-used to store all the correlated random values.
         effective_damageability (bool): if True, it uses effective damageability to draw damage samples instead of
           using the full monte carlo approach (i.e., to draw hazard intensity first, then damage).
         debug (int): for each random sample, print to the output stream the random loss (if 0),
           the random value used to draw the hazard intensity sample (if 1), the random value used to draw the damage sample (if 2).
         max_bytes_per_item (int): maximum bytes to be written in the output stream for an item.
-        buff_size (int): size in bytes of the output buffer.
-        int32_mv (numpy.ndarray): int32 view of the memoryview where the output is buffered.
-        cursor (int): index of int32_mv where to start writing.
+        byte_mv (numpy.array): byte view of where the output is buffered.
+        cursor (int): index of byte_mv where to start writing.
 
     Returns:
-        cursor (int): index of int32_mv where to start writing.
-        cursor_bytes (int): updated value of cursor_bytes, the cursor location in bytes.
+        cursor (int): index of byte_mv where to data has been written.
         last_processed_coverage_ids_idx (int): index of the last coverage_id stored in `coverage_ids` that was fully processed
           and printed to the output stream.
+        next_cached_vuln_cdf (int): index of the next free slot in the vuln cdf cache.
     """
     # loop through all the coverages that remain to be computed
     for coverage_i in range(last_processed_coverage_ids_idx, coverage_ids.shape[0]):
         coverage = coverages[coverage_ids[coverage_i]]
         tiv = coverage['tiv']
         Nitems = coverage['cur_items']
         exposureValue = tiv / Nitems
 
         # estimate max number of bytes needed to output this coverage
         # conservatively assume all random samples are printed (losses>loss_threshold)
-        cursor_bytes = cursor * int32_mv.itemsize
         est_cursor_bytes = Nitems * max_bytes_per_item
 
         # return before processing this coverage if the number of free bytes left in the buffer
         # is not sufficient to write out the full coverage
-        if cursor_bytes + est_cursor_bytes > buff_size:
-            return cursor, cursor_bytes, last_processed_coverage_ids_idx, next_cached_vuln_cdf
+        if cursor + est_cursor_bytes > byte_mv.shape[0]:
+            return cursor, last_processed_coverage_ids_idx, next_cached_vuln_cdf
 
         # compute losses for each item
         for item_j in range(Nitems):
             item_event_data = items_event_data[coverage['start_items'] + item_j]
             item_id = item_event_data['item_id']
             rng_index = item_event_data['rng_index']
             hazard_rng_index = item_event_data['hazard_rng_index']
@@ -967,25 +958,21 @@
         cursor = write_losses(event_id,
                               sample_size,
                               loss_threshold,
                               losses[:, :Nitems],
                               items_event_data[coverage['start_items']: coverage['start_items'] + Nitems]['item_id'],
                               alloc_rule,
                               tiv,
-                              int32_mv,
+                              byte_mv,
                               cursor)
 
         # register that another `coverage_id` has been processed
         last_processed_coverage_ids_idx += 1
 
-    # update cursor_bytes
-    cursor_bytes = cursor * int32_mv.itemsize
-
     return (cursor,
-            cursor_bytes,
             last_processed_coverage_ids_idx,
             next_cached_vuln_cdf)
 
 
 @njit(cache=True, fastmath=True)
 def get_vuln_cdf(vuln_i,
                  haz_int_bin_id,
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/gulpy.py` & `oasislmf-2.3.4/oasislmf/pytools/gulpy.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/modelpy.py` & `oasislmf-2.3.4/oasislmf/pytools/modelpy.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/pla/manager.py` & `oasislmf-2.3.4/oasislmf/pytools/pla/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .streams import read_and_write_streams
 from .structure import (
     get_items_amplifications,
     get_post_loss_amplification_factors
 )
 from oasis_data_manager.filestore.config import get_storage_from_config_path
 from oasislmf.pytools.utils import redirect_logging
+from oasislmf.pytools.common.event_stream import get_streams_in
 
 logger = logging.getLogger(__name__)
 
 
 @redirect_logging(exec_name='plapy')
 def run(
     run_dir, file_in, file_out, input_path, static_path, secondary_factor,
@@ -44,22 +45,19 @@
     items_amps = get_items_amplifications(input_path)
     plafactors = get_post_loss_amplification_factors(model_storage, secondary_factor, uniform_factor)
 
     # Set default factor should post loss amplification factor be missing
     default_factor = 1.0 if uniform_factor == 0.0 else uniform_factor
 
     with ExitStack() as stack:
-        if file_in is None:
-            stream_in = sys.stdin.buffer
-        else:
-            stream_in = stack.enter_context(open(file_in, 'rb'))
+        streams_in = get_streams_in(file_in, stack)
 
         if file_out is None:
             stream_out = sys.stdout.buffer
         else:
             stream_out = stack.enter_context(open(file_out, 'wb'))
 
         read_and_write_streams(
-            stream_in, stream_out, items_amps, plafactors, default_factor
+            streams_in, stream_out, items_amps, plafactors, default_factor
         )
 
     return 0
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/pla/structure.py` & `oasislmf-2.3.4/oasislmf/pytools/pla/structure.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/pytools/plapy.py` & `oasislmf-2.3.4/oasislmf/pytools/pla/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-from .pla import manager, logger
+from . import manager, logger
 
 import argparse
 import logging
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     '-f', '--secondary-factor',
```

### Comparing `oasislmf-2.3.2/oasislmf/pytools/utils.py` & `oasislmf-2.3.4/oasislmf/pytools/utils.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/calc_rules.py` & `oasislmf-2.3.4/oasislmf/utils/calc_rules.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/compress.py` & `oasislmf-2.3.4/oasislmf/utils/compress.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/coverages.py` & `oasislmf-2.3.4/oasislmf/utils/coverages.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/data.py` & `oasislmf-2.3.4/oasislmf/utils/data.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/defaults.py` & `oasislmf-2.3.4/oasislmf/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/diff.py` & `oasislmf-2.3.4/oasislmf/utils/diff.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/fm.py` & `oasislmf-2.3.4/oasislmf/utils/fm.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/inputs.py` & `oasislmf-2.3.4/oasislmf/utils/inputs.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/log.py` & `oasislmf-2.3.4/oasislmf/utils/log.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/path.py` & `oasislmf-2.3.4/oasislmf/utils/path.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/peril.py` & `oasislmf-2.3.4/oasislmf/utils/peril.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/profiles.py` & `oasislmf-2.3.4/oasislmf/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/utils/status.py` & `oasislmf-2.3.4/oasislmf/utils/status.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf/validation/model_data.py` & `oasislmf-2.3.4/oasislmf/validation/model_data.py`

 * *Files identical despite different names*

### Comparing `oasislmf-2.3.2/oasislmf.egg-info/PKG-INFO` & `oasislmf-2.3.4/oasislmf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasislmf
-Version: 2.3.2
+Version: 2.3.4
 Summary: Core loss modelling framework.
 Home-page: https://github.com/OasisLMF/oasislmf
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: BSD 3-Clause
 Keywords: oasis lmf loss modeling framework
 Platform: UNKNOWN
```

### Comparing `oasislmf-2.3.2/oasislmf.egg-info/SOURCES.txt` & `oasislmf-2.3.4/oasislmf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -82,34 +82,35 @@
 oasislmf/preparation/il_inputs.py
 oasislmf/preparation/lookup.py
 oasislmf/preparation/oed.py
 oasislmf/preparation/reinsurance_layer.py
 oasislmf/preparation/summaries.py
 oasislmf/pytools/__init__.py
 oasislmf/pytools/cdftocsv.py
-oasislmf/pytools/common.py
 oasislmf/pytools/compare_bin.py
 oasislmf/pytools/correlationtobin.py
 oasislmf/pytools/correlationtocsv.py
 oasislmf/pytools/dfcompare.py
-oasislmf/pytools/fmpy.py
 oasislmf/pytools/footprintconv.py
 oasislmf/pytools/gulpy.py
 oasislmf/pytools/modelpy.py
-oasislmf/pytools/plapy.py
 oasislmf/pytools/utils.py
+oasislmf/pytools/common/__init__.py
+oasislmf/pytools/common/data.py
+oasislmf/pytools/common/event_stream.py
 oasislmf/pytools/data_layer/__init__.py
 oasislmf/pytools/data_layer/footprint_layer.py
 oasislmf/pytools/data_layer/conversions/__init__.py
 oasislmf/pytools/data_layer/conversions/correlations.py
 oasislmf/pytools/data_layer/conversions/footprint.py
 oasislmf/pytools/data_layer/oasis_files/__init__.py
 oasislmf/pytools/data_layer/oasis_files/correlations.py
 oasislmf/pytools/fm/__init__.py
 oasislmf/pytools/fm/back_allocation.py
+oasislmf/pytools/fm/cli.py
 oasislmf/pytools/fm/common.py
 oasislmf/pytools/fm/compare.py
 oasislmf/pytools/fm/compute_sparse.py
 oasislmf/pytools/fm/financial_structure.py
 oasislmf/pytools/fm/manager.py
 oasislmf/pytools/fm/policy.py
 oasislmf/pytools/fm/policy_extras.py
@@ -129,18 +130,22 @@
 oasislmf/pytools/gulmc/__init__.py
 oasislmf/pytools/gulmc/aggregate.py
 oasislmf/pytools/gulmc/cli.py
 oasislmf/pytools/gulmc/common.py
 oasislmf/pytools/gulmc/items.py
 oasislmf/pytools/gulmc/manager.py
 oasislmf/pytools/pla/__init__.py
+oasislmf/pytools/pla/cli.py
 oasislmf/pytools/pla/common.py
 oasislmf/pytools/pla/manager.py
 oasislmf/pytools/pla/streams.py
 oasislmf/pytools/pla/structure.py
+oasislmf/pytools/summary/__init__.py
+oasislmf/pytools/summary/cli.py
+oasislmf/pytools/summary/manager.py
 oasislmf/utils/__init__.py
 oasislmf/utils/calc_rules.py
 oasislmf/utils/compress.py
 oasislmf/utils/coverages.py
 oasislmf/utils/data.py
 oasislmf/utils/defaults.py
 oasislmf/utils/diff.py
```

### Comparing `oasislmf-2.3.2/oasislmf.egg-info/entry_points.txt` & `oasislmf-2.3.4/oasislmf.egg-info/entry_points.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [console_scripts]
 complex_itemtobin = oasislmf.execution.complex_items_to_bin:main
 complex_itemtocsv = oasislmf.execution.complex_items_to_csv:main
 correlationtobin = oasislmf.pytools.correlationtobin:main
 correlationtocsv = oasislmf.pytools.correlationtocsv:main
 dfcompare = oasislmf.pytools.dfcompare:main
-fmpy = oasislmf.pytools.fmpy:main
+fmpy = oasislmf.pytools.fm.cli:main
 footprint_bin_to_parquet = oasislmf.pytools.data_layer.conversions.footprint:main
 footprint_compress = oasislmf.pytools.footprintconv:footprintconvpy
 gulmc = oasislmf.pytools.gulmc.cli:main
 gulpy = oasislmf.pytools.gulpy:main
 load_balancer = oasislmf.execution.load_balancer:main
 modelpy = oasislmf.pytools.modelpy:main
 oasislmf = oasislmf.cli.root:main
-plapy = oasislmf.pytools.plapy:main
+plapy = oasislmf.pytools.pla.cli:main
 servedata = oasislmf.pytools.data_layer.footprint_layer:main
+summarypy = oasislmf.pytools.summary.cli:main
 vulnerability_to_parquet = oasislmf.pytools.getmodel.vulnerability:main
 vulntoparquet = oasislmf.pytools.getmodel.vulnerability:main
```

### Comparing `oasislmf-2.3.2/setup.py` & `oasislmf-2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     from urllib import request as urlrequest
     from urllib.error import URLError
 except ImportError:
     from urllib2 import URLError
 
 
-KTOOLS_VERSION = '3.12.1'
+KTOOLS_VERSION = '3.12.2'
 
 SCRIPT_DIR = os.path.abspath(os.path.dirname(__file__))
 
 
 def get_readme():
     with io.open(os.path.join(SCRIPT_DIR, 'README.md'), encoding='utf-8') as readme:
         return readme.read()
@@ -374,22 +374,23 @@
             'complex_itemtocsv=oasislmf.execution.complex_items_to_csv:main',
             "vulnerability_to_parquet=oasislmf.pytools.getmodel.vulnerability:main",
             "footprint_bin_to_parquet=oasislmf.pytools.data_layer.conversions.footprint:main",
             'footprint_compress=oasislmf.pytools.footprintconv:footprintconvpy',
             "correlationtobin=oasislmf.pytools.correlationtobin:main",
             "correlationtocsv=oasislmf.pytools.correlationtocsv:main",
             'dfcompare=oasislmf.pytools.dfcompare:main',
-            'fmpy=oasislmf.pytools.fmpy:main',
+            'fmpy=oasislmf.pytools.fm.cli:main',
             'gulmc=oasislmf.pytools.gulmc.cli:main',
             'gulpy=oasislmf.pytools.gulpy:main',
             'load_balancer=oasislmf.execution.load_balancer:main',
             'modelpy=oasislmf.pytools.modelpy:main',
             'oasislmf=oasislmf.cli.root:main',
-            'plapy=oasislmf.pytools.plapy:main',
+            'plapy=oasislmf.pytools.pla.cli:main',
             "servedata=oasislmf.pytools.data_layer.footprint_layer:main",
+            'summarypy=oasislmf.pytools.summary.cli:main',
             'vulntoparquet=oasislmf.pytools.getmodel.vulnerability:main',
         ]
     },
     license='BSD 3-Clause',
     description='Core loss modelling framework.',
     long_description=readme,
     long_description_content_type='text/markdown',
```

