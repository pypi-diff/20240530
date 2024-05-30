# Comparing `tmp/palimpzest-0.1.8.tar.gz` & `tmp/palimpzest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palimpzest-0.1.8.tar", last modified: Thu May 30 00:36:09 2024, max compression
+gzip compressed data, was "palimpzest-0.1.9.tar", last modified: Thu May 30 00:44:36 2024, max compression
```

## Comparing `palimpzest-0.1.8.tar` & `palimpzest-0.1.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.751256 palimpzest-0.1.8/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-29 15:41:00.000000 palimpzest-0.1.8/LICENSE
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:36:09.751038 palimpzest-0.1.8/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-29 15:41:00.000000 palimpzest-0.1.8/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-30 00:36:06.000000 palimpzest-0.1.8/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-30 00:36:09.751300 palimpzest-0.1.8/setup.cfg
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.741714 palimpzest-0.1.8/src/
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.743041 palimpzest-0.1.8/src/cli/
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/cli/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/cli/cli_main.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.743508 palimpzest-0.1.8/src/palimpzest/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/__init__.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.744363 palimpzest-0.1.8/src/palimpzest/config/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/config/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/config/config.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/constants.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.744865 palimpzest-0.1.8/src/palimpzest/corelib/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/corelib/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/corelib/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/corelib/schemas.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.745083 palimpzest-0.1.8/src/palimpzest/datamanager/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/datamanager/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11011 2024-05-29 18:18:09.000000 palimpzest-0.1.8/src/palimpzest/datamanager/datamanager.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.745322 palimpzest-0.1.8/src/palimpzest/datasources/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/datasources/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4947 2024-05-29 23:32:36.000000 palimpzest-0.1.8/src/palimpzest/datasources/datasources.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/deploy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.746282 palimpzest-0.1.8/src/palimpzest/elements/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/elements/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/elements/aggregatefunction.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/elements/elements.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/elements/filters.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/elements/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/elements/groupbysig.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/elements/pzlist.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/elements/records.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.746499 palimpzest-0.1.8/src/palimpzest/execution/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      112 2024-05-29 01:56:02.000000 palimpzest-0.1.8/src/palimpzest/execution/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    18050 2024-05-30 00:35:51.000000 palimpzest-0.1.8/src/palimpzest/execution/execution.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.746811 palimpzest-0.1.8/src/palimpzest/generators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/generators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/generators/dspy_utils.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    25348 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/generators/generators.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.747354 palimpzest-0.1.8/src/palimpzest/operators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/operators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/operators/operators.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/operators/physical.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.747618 palimpzest-0.1.8/src/palimpzest/parallel/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/parallel/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/parallel/pzmodal.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.747909 palimpzest-0.1.8/src/palimpzest/policy/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/policy/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/policy/policy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.748531 palimpzest-0.1.8/src/palimpzest/profiler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/profiler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/profiler/attentive_trim.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/profiler/profiler.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/profiler/stats.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.748788 palimpzest-0.1.8/src/palimpzest/sampler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/sampler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/sampler/sampler.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.749019 palimpzest-0.1.8/src/palimpzest/sets/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/sets/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    14861 2024-05-29 18:07:06.000000 palimpzest-0.1.8/src/palimpzest/sets/sets.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.749756 palimpzest-0.1.8/src/palimpzest/solver/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/solver/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/solver/query_strategies.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/solver/solver.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-29 15:41:00.000000 palimpzest-0.1.8/src/palimpzest/solver/task_descriptors.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.750260 palimpzest-0.1.8/src/palimpzest/tools/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/tools/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/tools/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/tools/allenpdf.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/tools/pdfparser.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/tools/skema_tools.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.750625 palimpzest-0.1.8/src/palimpzest/utils/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/utils/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/utils/codegen.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.8/src/palimpzest/utils/sandbox.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:36:09.750808 palimpzest-0.1.8/src/palimpzest.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:36:09.000000 palimpzest-0.1.8/src/palimpzest.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-30 00:36:09.000000 palimpzest-0.1.8/src/palimpzest.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-30 00:36:09.000000 palimpzest-0.1.8/src/palimpzest.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-30 00:36:09.000000 palimpzest-0.1.8/src/palimpzest.egg-info/entry_points.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-30 00:36:09.000000 palimpzest-0.1.8/src/palimpzest.egg-info/requires.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-30 00:36:09.000000 palimpzest-0.1.8/src/palimpzest.egg-info/top_level.txt
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.640978 palimpzest-0.1.9/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-29 15:41:00.000000 palimpzest-0.1.9/LICENSE
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:44:36.640786 palimpzest-0.1.9/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-29 15:41:00.000000 palimpzest-0.1.9/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-30 00:44:27.000000 palimpzest-0.1.9/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-30 00:44:36.641010 palimpzest-0.1.9/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.631006 palimpzest-0.1.9/src/
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.632401 palimpzest-0.1.9/src/cli/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/cli/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/cli/cli_main.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.632898 palimpzest-0.1.9/src/palimpzest/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/__init__.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.633867 palimpzest-0.1.9/src/palimpzest/config/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/config/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/config/config.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/constants.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.634212 palimpzest-0.1.9/src/palimpzest/corelib/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/corelib/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/corelib/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/corelib/schemas.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.634480 palimpzest-0.1.9/src/palimpzest/datamanager/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/datamanager/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11011 2024-05-29 18:18:09.000000 palimpzest-0.1.9/src/palimpzest/datamanager/datamanager.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.634781 palimpzest-0.1.9/src/palimpzest/datasources/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/datasources/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4947 2024-05-29 23:32:36.000000 palimpzest-0.1.9/src/palimpzest/datasources/datasources.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/deploy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.635774 palimpzest-0.1.9/src/palimpzest/elements/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/elements/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/elements/aggregatefunction.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/elements/elements.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/elements/filters.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/elements/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/elements/groupbysig.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/elements/pzlist.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/elements/records.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.636015 palimpzest-0.1.9/src/palimpzest/execution/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      112 2024-05-29 01:56:02.000000 palimpzest-0.1.9/src/palimpzest/execution/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    16610 2024-05-30 00:44:17.000000 palimpzest-0.1.9/src/palimpzest/execution/execution.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.636389 palimpzest-0.1.9/src/palimpzest/generators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/generators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/generators/dspy_utils.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    25415 2024-05-30 00:44:15.000000 palimpzest-0.1.9/src/palimpzest/generators/generators.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.637103 palimpzest-0.1.9/src/palimpzest/operators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/operators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/operators/operators.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/operators/physical.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.637405 palimpzest-0.1.9/src/palimpzest/parallel/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/parallel/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/parallel/pzmodal.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.637646 palimpzest-0.1.9/src/palimpzest/policy/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/policy/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/policy/policy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.638168 palimpzest-0.1.9/src/palimpzest/profiler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/profiler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/profiler/attentive_trim.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/profiler/profiler.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/profiler/stats.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.638443 palimpzest-0.1.9/src/palimpzest/sampler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/sampler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/sampler/sampler.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.638673 palimpzest-0.1.9/src/palimpzest/sets/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/sets/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    14861 2024-05-29 18:07:06.000000 palimpzest-0.1.9/src/palimpzest/sets/sets.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.639396 palimpzest-0.1.9/src/palimpzest/solver/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/solver/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/solver/query_strategies.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/solver/solver.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-29 15:41:00.000000 palimpzest-0.1.9/src/palimpzest/solver/task_descriptors.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.640025 palimpzest-0.1.9/src/palimpzest/tools/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/tools/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/tools/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/tools/allenpdf.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/tools/pdfparser.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/tools/skema_tools.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.640413 palimpzest-0.1.9/src/palimpzest/utils/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/utils/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/utils/codegen.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.9/src/palimpzest/utils/sandbox.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:44:36.640571 palimpzest-0.1.9/src/palimpzest.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:44:36.000000 palimpzest-0.1.9/src/palimpzest.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-30 00:44:36.000000 palimpzest-0.1.9/src/palimpzest.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-30 00:44:36.000000 palimpzest-0.1.9/src/palimpzest.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-30 00:44:36.000000 palimpzest-0.1.9/src/palimpzest.egg-info/entry_points.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-30 00:44:36.000000 palimpzest-0.1.9/src/palimpzest.egg-info/requires.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-30 00:44:36.000000 palimpzest-0.1.9/src/palimpzest.egg-info/top_level.txt
```

### Comparing `palimpzest-0.1.8/LICENSE` & `palimpzest-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/PKG-INFO` & `palimpzest-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.8
+Version: 0.1.9
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.8/README.md` & `palimpzest-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/pyproject.toml` & `palimpzest-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "palimpzest"
-version = "0.1.8"
+version = "0.1.9"
 description = "Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["relational", "optimization", "llm", "AI programming", "extraction", "tools", "document", "search", "integration"]
 authors = [
     {name="MIT DSG Semantic Management Lab", email="michjc@csail.mit.edu"},
 ]
```

### Comparing `palimpzest-0.1.8/src/cli/cli_main.py` & `palimpzest-0.1.9/src/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/config/config.py` & `palimpzest-0.1.9/src/palimpzest/config/config.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/constants.py` & `palimpzest-0.1.9/src/palimpzest/constants.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/corelib/functions.py` & `palimpzest-0.1.9/src/palimpzest/corelib/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/corelib/schemas.py` & `palimpzest-0.1.9/src/palimpzest/corelib/schemas.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/datamanager/datamanager.py` & `palimpzest-0.1.9/src/palimpzest/datamanager/datamanager.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/datasources/datasources.py` & `palimpzest-0.1.9/src/palimpzest/datasources/datasources.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/elements/aggregatefunction.py` & `palimpzest-0.1.9/src/palimpzest/elements/aggregatefunction.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/elements/elements.py` & `palimpzest-0.1.9/src/palimpzest/elements/elements.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/elements/filters.py` & `palimpzest-0.1.9/src/palimpzest/elements/filters.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/elements/functions.py` & `palimpzest-0.1.9/src/palimpzest/elements/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/elements/groupbysig.py` & `palimpzest-0.1.9/src/palimpzest/elements/groupbysig.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/elements/pzlist.py` & `palimpzest-0.1.9/src/palimpzest/elements/pzlist.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/elements/records.py` & `palimpzest-0.1.9/src/palimpzest/elements/records.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/execution/execution.py` & `palimpzest-0.1.9/src/palimpzest/execution/execution.py`

 * *Files 14% similar despite different names*

```diff
@@ -331,34 +331,15 @@
                     raise Exception("No models available to create physical plans! You must set at least one of the following environment variables: [OPENAI_API_KEY, TOGETHER_API_KEY, GOOGLE_API_KEY]")
 
                 # find champion model plan records and add those to all_records
                 if (
                     all([model is None or model in [champion_model, "gpt-4-vision-preview"] for model in result_dict['plan_info']['models']])
                     and any([model == champion_model for model in result_dict['plan_info']['models']])
                 ):
-                    print("##############################")
-                    print("##############################")
-                    print("##############################")
-                    print(f"SETTING RETURN RECORDS -- {champion_model}")
-                    print(f"NUM RECORDS: {len(records)}")
-                    print(f"RECORDS: {records}")
                     return_records = records
-                    print(f"NUM RETURN RECORDS: {len(return_records)}")
-                    print(f"RETURN RECORDS: {return_records}")
-                    print("##############################")
-                    print("##############################")
-                    print("##############################")
-        
-        print("##############################")
-        print("##############################")
-        print("##############################")
-        print(f"RETURNING RETURN RECORDS: {return_records}")
-        print("##############################")
-        print("##############################")
-        print("##############################")
 
         return all_cost_estimate_data, return_records
 
 
     def __new__(cls, dataset: Set, policy: Policy, num_samples: int=20, nocache: bool=False, verbose: bool=False):
         # if nocache is True, make sure we do not re-use DSPy examples or codegen examples
         if nocache:
@@ -369,22 +350,14 @@
             # remove codegen samples from previous dataset from cache
             cache = DataDirectory().getCacheService()
             cache.rmCache()
 
         # TODO: if nocache=False and there is a cached result; don't run sentinels
         # run sentinel plans
         all_cost_estimate_data, sentinel_records = cls.run_sentinel_plans(dataset, num_samples, verbose)
-        print("##############################")
-        print("##############################")
-        print("##############################")
-        print(f"NUM SENTINEL RECORDS: {len(sentinel_records)}")
-        print(f"SENTINEL RECORDS: {sentinel_records}")
-        print("##############################")
-        print("##############################")
-        print("##############################")
 
         # create new plan candidates based on current estimate data
         logicalTree = dataset.getLogicalTree(nocache=nocache, scan_start_idx=num_samples)
         candidatePlans = logicalTree.createPhysicalPlanCandidates(
             cost_estimate_sample_data=all_cost_estimate_data,
             allow_model_selection=True,
             allow_codegen=True,
```

### Comparing `palimpzest-0.1.8/src/palimpzest/generators/dspy_utils.py` & `palimpzest-0.1.9/src/palimpzest/generators/dspy_utils.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/generators/generators.py` & `palimpzest-0.1.9/src/palimpzest/generators/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 # DEFINITIONS
 GenerationOutput = Tuple[str, GenerationStats]
 
 def get_api_key(key: str) -> str:
     # get API key from environment or throw an exception if it's not set
     if key not in os.environ:
+        print(f"KEY: {key}")
+        print(f"{os.environ.keys()}")
         raise ValueError(f"key not found in environment variables")
 
     return os.environ[key]
 
 
 class BaseGenerator:
     """
```

### Comparing `palimpzest-0.1.8/src/palimpzest/operators/operators.py` & `palimpzest-0.1.9/src/palimpzest/operators/operators.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/operators/physical.py` & `palimpzest-0.1.9/src/palimpzest/operators/physical.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/parallel/pzmodal.py` & `palimpzest-0.1.9/src/palimpzest/parallel/pzmodal.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/policy/policy.py` & `palimpzest-0.1.9/src/palimpzest/policy/policy.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/profiler/attentive_trim.py` & `palimpzest-0.1.9/src/palimpzest/profiler/attentive_trim.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/profiler/profiler.py` & `palimpzest-0.1.9/src/palimpzest/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/profiler/stats.py` & `palimpzest-0.1.9/src/palimpzest/profiler/stats.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/sets/sets.py` & `palimpzest-0.1.9/src/palimpzest/sets/sets.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/solver/query_strategies.py` & `palimpzest-0.1.9/src/palimpzest/solver/query_strategies.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/solver/solver.py` & `palimpzest-0.1.9/src/palimpzest/solver/solver.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/solver/task_descriptors.py` & `palimpzest-0.1.9/src/palimpzest/solver/task_descriptors.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/tools/allenpdf.py` & `palimpzest-0.1.9/src/palimpzest/tools/allenpdf.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/tools/pdfparser.py` & `palimpzest-0.1.9/src/palimpzest/tools/pdfparser.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/tools/skema_tools.py` & `palimpzest-0.1.9/src/palimpzest/tools/skema_tools.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/utils/codegen.py` & `palimpzest-0.1.9/src/palimpzest/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest/utils/sandbox.py` & `palimpzest-0.1.9/src/palimpzest/utils/sandbox.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest.egg-info/PKG-INFO` & `palimpzest-0.1.9/src/palimpzest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.8
+Version: 0.1.9
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.8/src/palimpzest.egg-info/SOURCES.txt` & `palimpzest-0.1.9/src/palimpzest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.8/src/palimpzest.egg-info/requires.txt` & `palimpzest-0.1.9/src/palimpzest.egg-info/requires.txt`

 * *Files identical despite different names*

