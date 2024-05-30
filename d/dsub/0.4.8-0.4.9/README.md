# Comparing `tmp/dsub-0.4.8.tar.gz` & `tmp/dsub-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsub-0.4.8.tar", last modified: Thu Dec 22 00:22:00 2022, max compression
+gzip compressed data, was "dsub-0.4.9.tar", last modified: Thu Apr 13 20:45:57 2023, max compression
```

## Comparing `dsub-0.4.8.tar` & `dsub-0.4.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.988300 dsub-0.4.8/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    11357 2022-12-22 00:21:40.000000 dsub-0.4.8/LICENSE
--rw-r--r--   0 willyn   (591014) primarygroup (89939)       96 2022-12-22 00:21:40.000000 dsub-0.4.8/MANIFEST.in
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    31966 2022-12-22 00:22:00.984300 dsub-0.4.8/PKG-INFO
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    31093 2022-12-22 00:21:40.000000 dsub-0.4.8/README.md
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.976299 dsub-0.4.8/dsub/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      678 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/__init__.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     1123 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/_dsub_version.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.976299 dsub-0.4.8/dsub/commands/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/commands/__init__.py
--rwxr-xr-x   0 willyn   (591014) primarygroup (89939)     6998 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/commands/ddel.py
--rwxr-xr-x   0 willyn   (591014) primarygroup (89939)    13363 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/commands/dstat.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    50478 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/commands/dsub.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.980299 dsub-0.4.8/dsub/lib/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/__init__.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     1292 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/dsub_errors.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    12686 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/dsub_util.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    32213 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/job_model.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    11339 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/output_formatter.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    39618 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/param_util.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     8611 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/providers_util.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     1579 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/resources.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     6091 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/lib/retry_util.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.980299 dsub-0.4.8/dsub/providers/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/__init__.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     8010 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/base.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     1208 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/batch_dummy.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    15696 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_base.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    22229 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_batch.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     7402 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_batch_operations.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     3409 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_cls_v2.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    15925 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_utils.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2221 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_v2.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    48816 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_v2_base.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    11455 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_v2_operations.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     8315 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_v2_pipelines.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      937 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/google_v2_versions.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.980299 dsub-0.4.8/dsub/providers/local/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     9009 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/local/runner.sh
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    37162 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/local.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     7837 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/provider_base.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     4944 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/stub.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2987 2022-12-22 00:21:40.000000 dsub-0.4.8/dsub/providers/test_fails.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.976299 dsub-0.4.8/dsub.egg-info/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    31966 2022-12-22 00:22:00.000000 dsub-0.4.8/dsub.egg-info/PKG-INFO
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     1973 2022-12-22 00:22:00.000000 dsub-0.4.8/dsub.egg-info/SOURCES.txt
--rw-r--r--   0 willyn   (591014) primarygroup (89939)        1 2022-12-22 00:22:00.000000 dsub-0.4.8/dsub.egg-info/dependency_links.txt
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      113 2022-12-22 00:22:00.000000 dsub-0.4.8/dsub.egg-info/entry_points.txt
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      366 2022-12-22 00:22:00.000000 dsub-0.4.8/dsub.egg-info/requires.txt
--rw-r--r--   0 willyn   (591014) primarygroup (89939)       10 2022-12-22 00:22:00.000000 dsub-0.4.8/dsub.egg-info/top_level.txt
--rw-r--r--   0 willyn   (591014) primarygroup (89939)       38 2022-12-22 00:22:00.988300 dsub-0.4.8/setup.cfg
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     4541 2022-12-22 00:21:40.000000 dsub-0.4.8/setup.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.980299 dsub-0.4.8/test/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2022-12-22 00:21:40.000000 dsub-0.4.8/test/__init__.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.984300 dsub-0.4.8/test/integration/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      623 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/__init__.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2294 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/e2e_after.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2475 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/e2e_after_fail.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2455 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/e2e_env_list.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     4739 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/e2e_io_tasks.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     8721 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/e2e_python_api.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     3928 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/get_data_value.py
--rwxr-xr-x   0 willyn   (591014) primarygroup (89939)      161 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/script_python.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2985 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/test_setup.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     6968 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/test_setup_e2e.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2626 2022-12-22 00:21:40.000000 dsub-0.4.8/test/integration/test_util.py
-drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2022-12-22 00:22:00.984300 dsub-0.4.8/test/unit/
--rw-r--r--   0 willyn   (591014) primarygroup (89939)       37 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/__init__.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      913 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/batch_client_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     1560 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/batch_handling_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     3242 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/custom_machine_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     4046 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/dstat_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     9893 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/dsub_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)      967 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/dsub_util_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2058 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/fake_time.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2596 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/fake_time_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    16388 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/job_model_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     3854 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/local_provider_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     5119 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/logging_uri_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)    19170 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/param_util_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     7859 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/retrying_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     1454 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/rfc3339_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     2356 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/stub_provider_test.py
--rw-r--r--   0 willyn   (591014) primarygroup (89939)     4348 2022-12-22 00:21:40.000000 dsub-0.4.8/test/unit/wait_and_retry_test.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.282408 dsub-0.4.9/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    11357 2023-04-13 20:45:40.000000 dsub-0.4.9/LICENSE
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)       96 2023-04-13 20:45:40.000000 dsub-0.4.9/MANIFEST.in
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    31966 2023-04-13 20:45:57.282408 dsub-0.4.9/PKG-INFO
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    31093 2023-04-13 20:45:40.000000 dsub-0.4.9/README.md
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.262406 dsub-0.4.9/dsub/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      678 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/__init__.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     1123 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/_dsub_version.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.270407 dsub-0.4.9/dsub/commands/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/commands/__init__.py
+-rwxr-xr-x   0 willyn   (591014) primarygroup (89939)     6998 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/commands/ddel.py
+-rwxr-xr-x   0 willyn   (591014) primarygroup (89939)    13363 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/commands/dstat.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    50478 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/commands/dsub.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.270407 dsub-0.4.9/dsub/lib/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/__init__.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     1292 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/dsub_errors.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    12686 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/dsub_util.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    32213 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/job_model.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    11339 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/output_formatter.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    39618 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/param_util.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     8611 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/providers_util.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     1579 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/resources.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     6091 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/lib/retry_util.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.274407 dsub-0.4.9/dsub/providers/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/__init__.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     8010 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/base.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     1240 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/batch_dummy.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    15696 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_base.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    29335 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_batch.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     8256 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_batch_operations.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     3409 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_cls_v2.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    15979 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_utils.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2221 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_v2.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    48977 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_v2_base.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    11455 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_v2_operations.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     8315 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_v2_pipelines.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      937 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/google_v2_versions.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.274407 dsub-0.4.9/dsub/providers/local/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     8716 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/local/runner.sh
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    37162 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/local.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     7837 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/provider_base.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     4944 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/stub.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2987 2023-04-13 20:45:40.000000 dsub-0.4.9/dsub/providers/test_fails.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.270407 dsub-0.4.9/dsub.egg-info/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    31966 2023-04-13 20:45:57.000000 dsub-0.4.9/dsub.egg-info/PKG-INFO
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     1973 2023-04-13 20:45:57.000000 dsub-0.4.9/dsub.egg-info/SOURCES.txt
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)        1 2023-04-13 20:45:57.000000 dsub-0.4.9/dsub.egg-info/dependency_links.txt
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      113 2023-04-13 20:45:57.000000 dsub-0.4.9/dsub.egg-info/entry_points.txt
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      367 2023-04-13 20:45:57.000000 dsub-0.4.9/dsub.egg-info/requires.txt
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)       10 2023-04-13 20:45:57.000000 dsub-0.4.9/dsub.egg-info/top_level.txt
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)       38 2023-04-13 20:45:57.282408 dsub-0.4.9/setup.cfg
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     4539 2023-04-13 20:45:40.000000 dsub-0.4.9/setup.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.274407 dsub-0.4.9/test/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      624 2023-04-13 20:45:40.000000 dsub-0.4.9/test/__init__.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.278407 dsub-0.4.9/test/integration/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      623 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/__init__.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2294 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/e2e_after.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2475 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/e2e_after_fail.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2455 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/e2e_env_list.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     4739 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/e2e_io_tasks.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     8721 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/e2e_python_api.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     3928 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/get_data_value.py
+-rwxr-xr-x   0 willyn   (591014) primarygroup (89939)      161 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/script_python.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2985 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/test_setup.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     7586 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/test_setup_e2e.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2626 2023-04-13 20:45:40.000000 dsub-0.4.9/test/integration/test_util.py
+drwxr-xr-x   0 willyn   (591014) primarygroup (89939)        0 2023-04-13 20:45:57.282408 dsub-0.4.9/test/unit/
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)       37 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/__init__.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      913 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/batch_client_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     1560 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/batch_handling_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     3242 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/custom_machine_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     4046 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/dstat_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     9893 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/dsub_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)      967 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/dsub_util_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2058 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/fake_time.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2596 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/fake_time_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    16388 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/job_model_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     3854 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/local_provider_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     5119 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/logging_uri_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)    19170 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/param_util_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     7859 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/retrying_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     1454 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/rfc3339_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     2356 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/stub_provider_test.py
+-rw-r--r--   0 willyn   (591014) primarygroup (89939)     4348 2023-04-13 20:45:40.000000 dsub-0.4.9/test/unit/wait_and_retry_test.py
```

### Comparing `dsub-0.4.8/LICENSE` & `dsub-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/PKG-INFO` & `dsub-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsub
-Version: 0.4.8
+Version: 0.4.9
 Summary: A command-line tool that makes it easy to submit and run batch scripts in the cloud
 Home-page: https://github.com/DataBiosphere/dsub
 Author: Verily
 License: Apache
 Keywords: cloud bioinformatics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dsub-0.4.8/README.md` & `dsub-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/__init__.py` & `dsub-0.4.9/dsub/__init__.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/_dsub_version.py` & `dsub-0.4.9/dsub/_dsub_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 The version should follow formatting requirements specified in PEP-440.
  - https://www.python.org/dev/peps/pep-0440
 
 A typical release sequence will be versioned as:
   0.1.3.dev0 -> 0.1.3 -> 0.1.4.dev0 -> ...
 """
 
-DSUB_VERSION = '0.4.8'
+DSUB_VERSION = '0.4.9'
```

### Comparing `dsub-0.4.8/dsub/commands/__init__.py` & `dsub-0.4.9/dsub/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/commands/ddel.py` & `dsub-0.4.9/dsub/commands/ddel.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/commands/dstat.py` & `dsub-0.4.9/dsub/commands/dstat.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/commands/dsub.py` & `dsub-0.4.9/dsub/commands/dsub.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/__init__.py` & `dsub-0.4.9/dsub/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/dsub_errors.py` & `dsub-0.4.9/dsub/lib/dsub_errors.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/dsub_util.py` & `dsub-0.4.9/dsub/lib/dsub_util.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/job_model.py` & `dsub-0.4.9/dsub/lib/job_model.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/output_formatter.py` & `dsub-0.4.9/dsub/lib/output_formatter.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/param_util.py` & `dsub-0.4.9/dsub/lib/param_util.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/providers_util.py` & `dsub-0.4.9/dsub/lib/providers_util.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/resources.py` & `dsub-0.4.9/dsub/lib/resources.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/lib/retry_util.py` & `dsub-0.4.9/dsub/lib/retry_util.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/__init__.py` & `dsub-0.4.9/dsub/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/base.py` & `dsub-0.4.9/dsub/providers/base.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/batch_dummy.py` & `dsub-0.4.9/dsub/providers/batch_dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 
 # pylint: disable=invalid-name
 class types(object):
   """Dummy docstring."""
   Job = None
   TaskGroup = None
-  LogsPolicy = None
   Volume = None
   TaskSpec = None
   Environment = None
 
   class task(object):
 
     class Runnable(object):
@@ -34,9 +33,12 @@
 
   class AllocationPolicy(object):
     InstancePolicyOrTemplate = None
     InstancePolicy = None
     AttachedDisk = None
     Disk = None
 
+  class LogsPolicy(object):
+    Destination = None
+
 
 # pylint: enable=invalid-name
```

### Comparing `dsub-0.4.8/dsub/providers/google_base.py` & `dsub-0.4.9/dsub/providers/google_base.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/google_batch_operations.py` & `dsub-0.4.9/dsub/providers/google_batch_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   return env_dict
 
 
 def is_done(op: batch_v1.types.Job) -> bool:
   """Return whether the operation has been marked done."""
   return op.status.state in [
       batch_v1.types.job.JobStatus.State.SUCCEEDED,
-      batch_v1.types.job.JobStatus.State.FAILED
+      batch_v1.types.job.JobStatus.State.FAILED,
   ]
 
 
 def is_success(op: batch_v1.types.Job) -> bool:
   """Return whether the operation has completed successfully."""
   return op.status.state == batch_v1.types.job.JobStatus.State.SUCCEEDED
 
@@ -94,45 +94,50 @@
     return None
 
 
 def get_status_events(op: batch_v1.types.Job):
   return op.status.status_events
 
 
-def build_job(task_groups: List[batch_v1.types.TaskGroup],
-              allocation_policy: batch_v1.types.AllocationPolicy,
-              labels: Dict[str, str],
-              logs_policy: batch_v1.types.LogsPolicy) -> batch_v1.types.Job:
+def build_job(
+    task_groups: List[batch_v1.types.TaskGroup],
+    allocation_policy: batch_v1.types.AllocationPolicy,
+    labels: Dict[str, str],
+    logs_policy: batch_v1.types.LogsPolicy,
+) -> batch_v1.types.Job:
   job = batch_v1.Job()
   job.task_groups = task_groups
   job.allocation_policy = allocation_policy
   job.labels = labels
   job.logs_policy = logs_policy
   return job
 
 
 def build_task_spec(
     runnables: List[batch_v1.types.task.Runnable],
-    volumes: List[batch_v1.types.Volume]) -> batch_v1.types.TaskSpec:
+    volumes: List[batch_v1.types.Volume],
+) -> batch_v1.types.TaskSpec:
   task_spec = batch_v1.TaskSpec()
   task_spec.runnables = runnables
   task_spec.volumes = volumes
   return task_spec
 
 
 def build_environment(env_vars: Dict[str, str]):
   environment = batch_v1.Environment()
   environment.variables = env_vars
   return environment
 
 
-def build_task_group(task_spec: batch_v1.types.TaskSpec,
-                     task_environments: List[batch_v1.types.Environment],
-                     task_count: int,
-                     task_count_per_node: int) -> batch_v1.types.TaskGroup:
+def build_task_group(
+    task_spec: batch_v1.types.TaskSpec,
+    task_environments: List[batch_v1.types.Environment],
+    task_count: int,
+    task_count_per_node: int,
+) -> batch_v1.types.TaskGroup:
   """Build a TaskGroup object for a Batch request.
 
   Args:
     task_spec (TaskSpec): TaskSpec object
     task_environments (List[Environment]): List of Environment objects
     task_count (int): The number of total tasks in the job
     task_count_per_node (int): The number of tasks to schedule on one VM
@@ -145,32 +150,54 @@
   task_group.task_environments = task_environments
   task_group.task_count = task_count
   task_group.task_count_per_node = task_count_per_node
   return task_group
 
 
 def build_container(
-    image_uri: str, entrypoint: str, volumes: List[str],
-    commands: List[str]) -> batch_v1.types.task.Runnable.Container:
+    image_uri: str, entrypoint: str, volumes: List[str], commands: List[str]
+) -> batch_v1.types.task.Runnable.Container:
   container = batch_v1.types.task.Runnable.Container()
   container.image_uri = image_uri
   container.entrypoint = entrypoint
   container.commands = commands
   container.volumes = volumes
   return container
 
 
-def build_runnable(image_uri: str, entrypoint: str, commands: List[str],
-                   run_in_background: bool, volumes: List[str],
-                   always_run: bool) -> batch_v1.types.task.Runnable:
+def build_runnable(
+    run_in_background: bool,
+    always_run: bool,
+    environment: batch_v1.types.Environment,
+    image_uri: str,
+    entrypoint: str,
+    volumes: List[str],
+    commands: List[str],
+) -> batch_v1.types.task.Runnable:
+  """Build a Runnable object for a Batch request.
+
+  Args:
+    run_in_background (bool): True for the action to run in the background
+    always_run (bool): True for the action to run even in case of error from
+      prior actions
+    environment (Environment): Environment variables for action
+    image_uri (str): Docker image path
+    entrypoint (str): Docker image entrypoint path
+    volumes (List[str]): List of volume mounts (host_path:container_path)
+    commands (List[str]): Command arguments to pass to the entrypoint
+
+  Returns:
+    An object representing a Runnable
+  """
   container = build_container(image_uri, entrypoint, volumes, commands)
   runnable = batch_v1.Runnable()
   runnable.container = container
   runnable.background = run_in_background
   runnable.always_run = always_run
+  runnable.environment = environment
   return runnable
 
 
 def build_volume(disk: str, path: str) -> batch_v1.types.Volume:
   """Build a Volume object for a Batch request.
 
   Args:
@@ -183,45 +210,56 @@
   volume = batch_v1.Volume()
   volume.device_name = disk
   volume.mount_path = path
   return volume
 
 
 def build_allocation_policy(
-    ipts: List[batch_v1.types.AllocationPolicy.InstancePolicyOrTemplate]
+    ipts: List[batch_v1.types.AllocationPolicy.InstancePolicyOrTemplate],
 ) -> batch_v1.types.AllocationPolicy:
   allocation_policy = batch_v1.AllocationPolicy()
   allocation_policy.instances = ipts
   return allocation_policy
 
 
 def build_instance_policy_or_template(
-    instance_policy: batch_v1.types.AllocationPolicy.InstancePolicy
+    instance_policy: batch_v1.types.AllocationPolicy.InstancePolicy,
 ) -> batch_v1.types.AllocationPolicy.InstancePolicyOrTemplate:
   ipt = batch_v1.AllocationPolicy.InstancePolicyOrTemplate()
   ipt.policy = instance_policy
   return ipt
 
 
+def build_logs_policy(
+    destination: batch_v1.types.LogsPolicy.Destination, logs_path: str
+) -> batch_v1.types.LogsPolicy:
+  logs_policy = batch_v1.LogsPolicy()
+  logs_policy.destination = destination
+  logs_policy.logs_path = logs_path
+
+  return logs_policy
+
+
 def build_instance_policy(
-    disks: List[batch_v1.types.AllocationPolicy.AttachedDisk]
+    disks: List[batch_v1.types.AllocationPolicy.AttachedDisk],
 ) -> batch_v1.types.AllocationPolicy.InstancePolicy:
   instance_policy = batch_v1.AllocationPolicy.InstancePolicy()
   instance_policy.disks = [disks]
   return instance_policy
 
 
 def build_attached_disk(
-    disk: batch_v1.types.AllocationPolicy.Disk,
-    device_name: str) -> batch_v1.types.AllocationPolicy.AttachedDisk:
+    disk: batch_v1.types.AllocationPolicy.Disk, device_name: str
+) -> batch_v1.types.AllocationPolicy.AttachedDisk:
   attached_disk = batch_v1.AllocationPolicy.AttachedDisk()
   attached_disk.new_disk = disk
   attached_disk.device_name = device_name
   return attached_disk
 
 
 def build_persistent_disk(
-    size_gb: int, disk_type: str) -> batch_v1.types.AllocationPolicy.Disk:
+    size_gb: int, disk_type: str
+) -> batch_v1.types.AllocationPolicy.Disk:
   disk = batch_v1.AllocationPolicy.Disk()
   disk.type = disk_type
   disk.size_gb = size_gb
   return disk
```

### Comparing `dsub-0.4.8/dsub/providers/google_cls_v2.py` & `dsub-0.4.9/dsub/providers/google_cls_v2.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/google_utils.py` & `dsub-0.4.9/dsub/providers/google_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,17 @@
         sleep 10s
       fi
     done
 
     log_error "gsutil ${headers} ${user_project_flag} -mq cp \"${src}\" \"${dst}\""
     exit 1
   }
+""")
+
+LOG_CP_FN = GSUTIL_CP_FN + textwrap.dedent("""\
 
   function log_cp() {
     local src="${1}"
     local dst="${2}"
     local tmp="${3}"
     local check_src="${4}"
     local user_project_name="${5}"
```

### Comparing `dsub-0.4.8/dsub/providers/google_v2.py` & `dsub-0.4.9/dsub/providers/google_v2.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/google_v2_base.py` & `dsub-0.4.9/dsub/providers/google_v2_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
   LOG_PID=$!
 
   wait "${{STDOUT_PID}}"
   wait "${{STDERR_PID}}"
   wait "${{LOG_PID}}"
 """)
 
-_LOGGING_CMD = textwrap.dedent("""\
+_FINAL_LOGGING_CMD = textwrap.dedent("""\
   set -o errexit
   set -o nounset
   set -o pipefail
 
   {log_msg_fn}
   {log_cp_fn}
   {log_cp_cmd}
@@ -421,27 +421,30 @@
     mount_actions = self._get_mount_actions(gcs_mounts, mnt_datadisk)
     optional_actions += len(mount_actions)
 
     user_action = 4 + optional_actions
     final_logging_action = 6 + optional_actions
 
     # Set up the commands and environment for the logging actions
-    logging_cmd = _LOGGING_CMD.format(
+    final_logging_cmd = _FINAL_LOGGING_CMD.format(
         log_msg_fn=google_utils.LOG_MSG_FN,
-        log_cp_fn=google_utils.GSUTIL_CP_FN,
+        log_cp_fn=google_utils.LOG_CP_FN,
         log_cp_cmd=_LOG_CP_CMD.format(
-            user_action=user_action, logging_action='logging_action'))
+            user_action=user_action, logging_action='logging_action'
+        ),
+    )
     continuous_logging_cmd = _CONTINUOUS_LOGGING_CMD.format(
         log_msg_fn=google_utils.LOG_MSG_FN,
-        log_cp_fn=google_utils.GSUTIL_CP_FN,
+        log_cp_fn=google_utils.LOG_CP_FN,
         log_cp_cmd=_LOG_CP_CMD.format(
-            user_action=user_action,
-            logging_action='continuous_logging_action'),
+            user_action=user_action, logging_action='continuous_logging_action'
+        ),
         final_logging_action=final_logging_action,
-        log_interval=job_resources.log_interval or '60s')
+        log_interval=job_resources.log_interval or '60s',
+    )
     logging_env = self._get_logging_env(task_resources.logging_path.uri,
                                         user_project)
 
     # Set up command and environments for the prepare, localization, user,
     # and de-localization actions
     script_path = os.path.join(_SCRIPT_DIR, script.name)
     prepare_command = google_utils.PREPARE_CMD.format(
@@ -510,55 +513,64 @@
             entrypoint='/bin/bash',
             commands=[
                 '-c',
                 google_utils.LOCALIZATION_CMD.format(
                     log_msg_fn=google_utils.LOG_MSG_FN,
                     recursive_cp_fn=google_utils.GSUTIL_RSYNC_FN,
                     cp_fn=google_utils.GSUTIL_CP_FN,
-                    cp_loop=google_utils.LOCALIZATION_LOOP)
-            ]),
+                    cp_loop=google_utils.LOCALIZATION_LOOP,
+                ),
+            ],
+        ),
         google_v2_pipelines.build_action(
             name='user-command',
             pid_namespace=pid_namespace,
             block_external_network=job_resources.block_external_network,
             image_uri=job_resources.image,
-            mounts=[mnt_datadisk] + persistent_disk_mounts +
-            existing_disk_mounts,
+            mounts=[mnt_datadisk]
+            + persistent_disk_mounts
+            + existing_disk_mounts,
             environment=user_environment,
             entrypoint='/usr/bin/env',
             commands=[
-                'bash', '-c',
+                'bash',
+                '-c',
                 google_utils.USER_CMD.format(
                     tmp_dir=_TMP_DIR,
                     working_dir=_WORKING_DIR,
-                    user_script=script_path)
-            ]),
+                    user_script=script_path,
+                ),
+            ],
+        ),
         google_v2_pipelines.build_action(
             name='delocalization',
             pid_namespace=pid_namespace,
             image_uri=google_utils.CLOUD_SDK_IMAGE,
             mounts=[mnt_datadisk],
             environment=delocalization_env,
             entrypoint='/bin/bash',
             commands=[
                 '-c',
                 google_utils.LOCALIZATION_CMD.format(
                     log_msg_fn=google_utils.LOG_MSG_FN,
                     recursive_cp_fn=google_utils.GSUTIL_RSYNC_FN,
                     cp_fn=google_utils.GSUTIL_CP_FN,
-                    cp_loop=google_utils.DELOCALIZATION_LOOP)
-            ]),
+                    cp_loop=google_utils.DELOCALIZATION_LOOP,
+                ),
+            ],
+        ),
         google_v2_pipelines.build_action(
             name='final_logging',
             pid_namespace=pid_namespace,
             always_run=True,
             image_uri=google_utils.CLOUD_SDK_IMAGE,
             environment=logging_env,
             entrypoint='/bin/bash',
-            commands=['-c', logging_cmd]),
+            commands=['-c', final_logging_cmd],
+        ),
     ])
 
     assert len(actions) - 2 == user_action
     assert len(actions) == final_logging_action
 
     # Prepare the VM (resources) configuration
     volumes = [
```

### Comparing `dsub-0.4.8/dsub/providers/google_v2_operations.py` & `dsub-0.4.9/dsub/providers/google_v2_operations.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/google_v2_pipelines.py` & `dsub-0.4.9/dsub/providers/google_v2_pipelines.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/google_v2_versions.py` & `dsub-0.4.9/dsub/providers/google_v2_versions.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/local/runner.sh` & `dsub-0.4.9/dsub/providers/local/runner.sh`

 * *Files 3% similar despite different names*

```diff
@@ -141,46 +141,28 @@
     log_error "${message} on or near line ${parent_lineno}; ${0} exiting with status ${code}"
   fi
   cleanup "false"
   exit "${code}"
 }
 readonly -f error
 
-function fetch_image() {
-  local image="$1"
-
-  for ((attempt=0; attempt < 3; attempt++)); do
-    log_info "Using gcloud to fetch ${image}."
-    if gcloud docker -- pull "${image}"; then
-      return
-    fi
-    if (( attempt < 2 )); then
-      log_info "Sleeping 30s before the next attempt."
-      sleep 30s
-    fi
-  done
-
-  log_error "FAILED to fetch ${image}"
-  exit 1
-}
-readonly -f fetch_image
-
-function fetch_image_if_necessary() {
+function configure_docker_if_necessary() {
   local image="$1"
 
   # Remove everything from the first / on
   local prefix="${image%%/*}"
 
   # Check that the prefix is gcr.io or <location>.gcr.io
   if [[ "${prefix}" == "gcr.io" ]] ||
      [[ "${prefix}" == *.gcr.io ]]; then
-    fetch_image "${image}"
+    log_info "Ensuring docker auth is configured for ${prefix}"
+    gcloud --quiet auth configure-docker "${prefix}"
   fi
 }
-readonly -f fetch_image_if_necessary
+readonly -f configure_docker_if_necessary
 
 function get_docker_user() {
   # Get the userid and groupid the Docker image is set to run as.
   docker run \
     --name "${NAME}-get-docker-userid" \
     --entrypoint /usr/bin/env \
     "${IMAGE}" \
@@ -243,15 +225,15 @@
 # Make sure that ERR traps are inherited by shell functions
 set -o errtrace
 
 write_event "start"
 
 # Handle gcr.io images
 write_event "pulling-image"
-fetch_image_if_necessary "${IMAGE}"
+configure_docker_if_necessary "${IMAGE}"
 
 # Copy inputs
 cd "${TASK_DIR}"
 write_event "localizing-files"
 write_status "RUNNING"
 log_info "Localizing inputs."
 localize_data
```

### Comparing `dsub-0.4.8/dsub/providers/local.py` & `dsub-0.4.9/dsub/providers/local.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/provider_base.py` & `dsub-0.4.9/dsub/providers/provider_base.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/stub.py` & `dsub-0.4.9/dsub/providers/stub.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub/providers/test_fails.py` & `dsub-0.4.9/dsub/providers/test_fails.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/dsub.egg-info/PKG-INFO` & `dsub-0.4.9/dsub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsub
-Version: 0.4.8
+Version: 0.4.9
 Summary: A command-line tool that makes it easy to submit and run batch scripts in the cloud
 Home-page: https://github.com/DataBiosphere/dsub
 Author: Verily
 License: Apache
 Keywords: cloud bioinformatics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dsub-0.4.8/dsub.egg-info/SOURCES.txt` & `dsub-0.4.9/dsub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/setup.py` & `dsub-0.4.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,33 @@
 from setuptools import setup
 
 
 _DEPENDENCIES = [
     # dependencies for dsub, ddel, dstat
     # Pin to known working versions to prevent episodic breakage from library
     # version mismatches.
-    # This version list generated: 12/15/2022
-
+    # This version list generated: 04/13/2023
     # direct dependencies
-    'google-api-python-client>=2.47.0,<=2.70.0',
-    'google-auth>=2.6.6,<=2.15.0',
-    'google-cloud-batch==0.6.0',
+    'google-api-python-client>=2.47.0,<=2.85.0',
+    'google-auth>=2.6.6,<=2.17.3',
+    'google-cloud-batch==0.10.0',
     'python-dateutil<=2.8.2',
-    'pytz<=2022.7',
+    'pytz<=2023.3',
     'pyyaml<=6.0',
-    'tenacity<=7.0.0',
-    'tabulate<=0.8.9',
-
+    'tenacity<=8.2.2',
+    'tabulate<=0.9.0',
     # downstream dependencies
     'funcsigs==1.0.2',
     'google-api-core>=2.7.3,<=2.11.0',
     'google-auth-httplib2<=0.1.0',
-    'httplib2<=0.21.0',
+    'httplib2<=0.22.0',
     'pyasn1<=0.4.8',
     'pyasn1-modules<=0.2.8',
     'rsa<=4.9',
     'uritemplate<=4.1.1',
-
     # dependencies for test code
     'parameterized<=0.8.1',
     'mock<=4.0.3',
 ]
 
 
 def unittest_suite():
```

### Comparing `dsub-0.4.8/test/__init__.py` & `dsub-0.4.9/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/__init__.py` & `dsub-0.4.9/test/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/e2e_after.py` & `dsub-0.4.9/test/integration/e2e_after.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/e2e_after_fail.py` & `dsub-0.4.9/test/integration/e2e_after_fail.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/e2e_env_list.py` & `dsub-0.4.9/test/integration/e2e_env_list.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/e2e_io_tasks.py` & `dsub-0.4.9/test/integration/e2e_io_tasks.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/e2e_python_api.py` & `dsub-0.4.9/test/integration/e2e_python_api.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/get_data_value.py` & `dsub-0.4.9/test/integration/get_data_value.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/test_setup.py` & `dsub-0.4.9/test/integration/test_setup.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/integration/test_setup_e2e.py` & `dsub-0.4.9/test/integration/test_setup_e2e.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,39 @@
 
 
 def run_dsub(dsub_args):
   # Execute the appropriate dsub_<provider> function
   return globals()["dsub_%s" % DSUB_PROVIDER.replace("-", "_")](dsub_args)
 
 
+def dsub_google_batch(dsub_args):
+  """Call dsub appending google-batch required arguments."""
+  # pyformat: disable
+  google_batch_opt_args = [
+      ("BOOT_DISK_SIZE", "--boot-disk-size"),
+      ("DISK_SIZE", "--disk-size")
+  ]
+  # pyformat: enable
+
+  opt_args = []
+  for var in google_batch_opt_args:
+    val = globals().get(var[0])
+    if val:
+      opt_args.append(var[1], val)
+
+  # pyformat: disable
+  return dsub_command.call([
+      "--provider", "google-batch",
+      "--project", PROJECT_ID,
+      "--logging", LOGGING,
+      "--regions", "us-central1"
+      ] + opt_args + dsub_args)
+  # pyformat: enable
+
+
 def dsub_google_cls_v2(dsub_args):
   """Call dsub appending google-cls-v2 required arguments."""
   # pyformat: disable
   google_cls_v2_opt_args = [
       ("BOOT_DISK_SIZE", "--boot-disk-size"),
       ("DISK_SIZE", "--disk-size")
   ]
```

### Comparing `dsub-0.4.8/test/integration/test_util.py` & `dsub-0.4.9/test/integration/test_util.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/batch_client_test.py` & `dsub-0.4.9/test/unit/batch_client_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/batch_handling_test.py` & `dsub-0.4.9/test/unit/batch_handling_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/custom_machine_test.py` & `dsub-0.4.9/test/unit/custom_machine_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/dstat_test.py` & `dsub-0.4.9/test/unit/dstat_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/dsub_test.py` & `dsub-0.4.9/test/unit/dsub_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/dsub_util_test.py` & `dsub-0.4.9/test/unit/dsub_util_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/fake_time.py` & `dsub-0.4.9/test/unit/fake_time.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/fake_time_test.py` & `dsub-0.4.9/test/unit/fake_time_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/job_model_test.py` & `dsub-0.4.9/test/unit/job_model_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/local_provider_test.py` & `dsub-0.4.9/test/unit/local_provider_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/logging_uri_test.py` & `dsub-0.4.9/test/unit/logging_uri_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/param_util_test.py` & `dsub-0.4.9/test/unit/param_util_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/retrying_test.py` & `dsub-0.4.9/test/unit/retrying_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/rfc3339_test.py` & `dsub-0.4.9/test/unit/rfc3339_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/stub_provider_test.py` & `dsub-0.4.9/test/unit/stub_provider_test.py`

 * *Files identical despite different names*

### Comparing `dsub-0.4.8/test/unit/wait_and_retry_test.py` & `dsub-0.4.9/test/unit/wait_and_retry_test.py`

 * *Files identical despite different names*

