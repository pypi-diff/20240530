# Comparing `tmp/crunch_cli-3.9.2.tar.gz` & `tmp/crunch_cli-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch_cli-3.9.2.tar", last modified: Tue May 14 14:22:17 2024, max compression
+gzip compressed data, was "crunch_cli-3.9.3.tar", last modified: Thu May 30 11:50:04 2024, max compression
```

## Comparing `crunch_cli-3.9.2.tar` & `crunch_cli-3.9.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.783110 crunch_cli-3.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-14 14:22:17.783110 crunch_cli-3.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.767110 crunch_cli-3.9.2/crunch/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.771110 crunch_cli-3.9.2/crunch/api/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.775110 crunch_cli-3.9.2/crunch/api/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/competition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/crunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/data_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/enum_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/quickstarter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/round.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/domain/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/api/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.775110 crunch_cli-3.9.2/crunch/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/benchmark/orthogonalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.775110 crunch_cli-3.9.2/crunch/checker/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/checker/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/checker/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.775110 crunch_cli-3.9.2/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/quickstarter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/command/update_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/monkey_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.775110 crunch_cli-3.9.2/crunch/orthogonalization/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/orthogonalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/orthogonalization/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/orthogonalization/orthogonalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.779110 crunch_cli-3.9.2/crunch/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/runner/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/runner/cloud_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/runner/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/runner/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.779110 crunch_cli-3.9.2/crunch/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/scoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.779110 crunch_cli-3.9.2/crunch/scoring/_format/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/scoring/_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/scoring/_format/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/scoring/_format/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/scoring/reducers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/scoring/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/scoring/scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/store.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.779110 crunch_cli-3.9.2/crunch/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch/vendor/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/crunch-monkeypatch.pth
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:22:17.779110 crunch_cli-3.9.2/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-14 14:22:17.000000 crunch_cli-3.9.2/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-14 14:22:17.000000 crunch_cli-3.9.2/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:22:17.000000 crunch_cli-3.9.2/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 14:22:17.000000 crunch_cli-3.9.2/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:22:17.000000 crunch_cli-3.9.2/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-14 14:22:17.000000 crunch_cli-3.9.2/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 14:22:17.000000 crunch_cli-3.9.2/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:22:17.783110 crunch_cli-3.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 14:22:08.000000 crunch_cli-3.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.706208 crunch_cli-3.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-30 11:50:04.706208 crunch_cli-3.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.690208 crunch_cli-3.9.3/crunch/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.694208 crunch_cli-3.9.3/crunch/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.698208 crunch_cli-3.9.3/crunch/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/competition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/crunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/data_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/enum_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/quickstarter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/round.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/domain/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/api/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.698208 crunch_cli-3.9.3/crunch/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/benchmark/orthogonalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.698208 crunch_cli-3.9.3/crunch/checker/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/checker/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/checker/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.698208 crunch_cli-3.9.3/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/quickstarter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/command/update_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/monkey_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.698208 crunch_cli-3.9.3/crunch/orthogonalization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/orthogonalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/orthogonalization/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/orthogonalization/orthogonalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.702208 crunch_cli-3.9.3/crunch/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17817 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/runner/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13908 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/runner/cloud_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/runner/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.702208 crunch_cli-3.9.3/crunch/scoring/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/scoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.702208 crunch_cli-3.9.3/crunch/scoring/_format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/scoring/_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/scoring/_format/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/scoring/_format/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/scoring/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/scoring/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/scoring/scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.702208 crunch_cli-3.9.3/crunch/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch/vendor/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/crunch-monkeypatch.pth
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:50:04.706208 crunch_cli-3.9.3/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-30 11:50:04.000000 crunch_cli-3.9.3/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-30 11:50:04.000000 crunch_cli-3.9.3/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:50:04.000000 crunch_cli-3.9.3/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 11:50:04.000000 crunch_cli-3.9.3/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:50:04.000000 crunch_cli-3.9.3/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 11:50:04.000000 crunch_cli-3.9.3/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 11:50:04.000000 crunch_cli-3.9.3/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:50:04.706208 crunch_cli-3.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-30 11:50:01.000000 crunch_cli-3.9.3/setup.py
```

### Comparing `crunch_cli-3.9.2/PKG-INFO` & `crunch_cli-3.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch-cli
-Version: 3.9.2
+Version: 3.9.3
 Summary: crunch-cli - CLI of the CrunchDAO Platform
 Home-page: https://github.com/crunchdao/crunch-cli
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crunch_cli-3.9.2/README.md` & `crunch_cli-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/auth.py` & `crunch_cli-3.9.3/crunch/api/auth.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/client.py` & `crunch_cli-3.9.3/crunch/api/client.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/__init__.py` & `crunch_cli-3.9.3/crunch/api/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/check.py` & `crunch_cli-3.9.3/crunch/api/domain/check.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/competition.py` & `crunch_cli-3.9.3/crunch/api/domain/competition.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/crunch.py` & `crunch_cli-3.9.3/crunch/api/domain/crunch.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/data_release.py` & `crunch_cli-3.9.3/crunch/api/domain/data_release.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/library.py` & `crunch_cli-3.9.3/crunch/api/domain/library.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/metric.py` & `crunch_cli-3.9.3/crunch/api/domain/metric.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/phase.py` & `crunch_cli-3.9.3/crunch/api/domain/phase.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/prediction.py` & `crunch_cli-3.9.3/crunch/api/domain/prediction.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/project.py` & `crunch_cli-3.9.3/crunch/api/domain/project.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/quickstarter.py` & `crunch_cli-3.9.3/crunch/api/domain/quickstarter.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/round.py` & `crunch_cli-3.9.3/crunch/api/domain/round.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/run.py` & `crunch_cli-3.9.3/crunch/api/domain/run.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/runner.py` & `crunch_cli-3.9.3/crunch/api/domain/runner.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/score.py` & `crunch_cli-3.9.3/crunch/api/domain/score.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/submission.py` & `crunch_cli-3.9.3/crunch/api/domain/submission.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/domain/user.py` & `crunch_cli-3.9.3/crunch/api/domain/user.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/errors.py` & `crunch_cli-3.9.3/crunch/api/errors.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/identifiers.py` & `crunch_cli-3.9.3/crunch/api/identifiers.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/api/resource.py` & `crunch_cli-3.9.3/crunch/api/resource.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/benchmark/orthogonalization.py` & `crunch_cli-3.9.3/crunch/benchmark/orthogonalization.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/checker/checker.py` & `crunch_cli-3.9.3/crunch/checker/checker.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/checker/functions.py` & `crunch_cli-3.9.3/crunch/checker/functions.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/cli.py` & `crunch_cli-3.9.3/crunch/cli.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/command/convert.py` & `crunch_cli-3.9.3/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/command/download.py` & `crunch_cli-3.9.3/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/command/push.py` & `crunch_cli-3.9.3/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/command/quickstarter.py` & `crunch_cli-3.9.3/crunch/command/quickstarter.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/command/setup.py` & `crunch_cli-3.9.3/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/command/test.py` & `crunch_cli-3.9.3/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/constants.py` & `crunch_cli-3.9.3/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/ensure.py` & `crunch_cli-3.9.3/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/inline.py` & `crunch_cli-3.9.3/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/library.py` & `crunch_cli-3.9.3/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/monkey_patches.py` & `crunch_cli-3.9.3/crunch/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/orthogonalization/__init__.py` & `crunch_cli-3.9.3/crunch/orthogonalization/__init__.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/orthogonalization/orthogonalize.py` & `crunch_cli-3.9.3/crunch/orthogonalization/orthogonalize.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/runner/cloud.py` & `crunch_cli-3.9.3/crunch/runner/cloud.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/runner/cloud_executor.py` & `crunch_cli-3.9.3/crunch/runner/cloud_executor.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/runner/local.py` & `crunch_cli-3.9.3/crunch/runner/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,17 @@
 
         return (
             self.keys,
             False,
         )
 
     def start_dag(self):
-        x_train = utils.read(self.x_train_path, dataframe=False, kwargs=self.read_kwargs)
-        x_test = utils.read(self.x_test_path, dataframe=False, kwargs=self.read_kwargs)
-        y_train = utils.read(self.y_train_path, dataframe=False, kwargs=self.read_kwargs)
+        x_train = utils.read(self.x_train_path, kwargs=self.read_kwargs)
+        x_test = utils.read(self.x_test_path, kwargs=self.read_kwargs)
+        y_train = utils.read(self.y_train_path, kwargs=self.read_kwargs)
 
         default_values = {
             "number_of_features": self.number_of_features,
             "model_directory_path": self.model_directory_path,
             "id_column_name": self.column_names.id,
             "prediction_column_name": self.column_names.prediction,
             "column_names": self.column_names,
```

### Comparing `crunch_cli-3.9.2/crunch/runner/runner.py` & `crunch_cli-3.9.3/crunch/runner/runner.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/scoring/_format/dag.py` & `crunch_cli-3.9.3/crunch/scoring/_format/dag.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/scoring/_format/timeseries.py` & `crunch_cli-3.9.3/crunch/scoring/_format/timeseries.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/scoring/score.py` & `crunch_cli-3.9.3/crunch/scoring/score.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/scoring/scorers.py` & `crunch_cli-3.9.3/crunch/scoring/scorers.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/store.py` & `crunch_cli-3.9.3/crunch/store.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/tester.py` & `crunch_cli-3.9.3/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/utils.py` & `crunch_cli-3.9.3/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/vendor/__init__.py` & `crunch_cli-3.9.3/crunch/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch/vendor/datacrunch.py` & `crunch_cli-3.9.3/crunch/vendor/datacrunch.py`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/crunch_cli.egg-info/PKG-INFO` & `crunch_cli-3.9.3/crunch_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crunch-cli
-Version: 3.9.2
+Version: 3.9.3
 Summary: crunch-cli - CLI of the CrunchDAO Platform
 Home-page: https://github.com/crunchdao/crunch-cli
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crunch_cli-3.9.2/crunch_cli.egg-info/SOURCES.txt` & `crunch_cli-3.9.3/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch_cli-3.9.2/setup.py` & `crunch_cli-3.9.3/setup.py`

 * *Files identical despite different names*

