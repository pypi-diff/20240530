# Comparing `tmp/palimpzest-0.1.5.tar.gz` & `tmp/palimpzest-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palimpzest-0.1.5.tar", last modified: Thu May 30 00:07:11 2024, max compression
+gzip compressed data, was "palimpzest-0.1.6.tar", last modified: Thu May 30 00:12:06 2024, max compression
```

## Comparing `palimpzest-0.1.5.tar` & `palimpzest-0.1.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.878280 palimpzest-0.1.5/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-29 15:41:00.000000 palimpzest-0.1.5/LICENSE
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:07:11.878077 palimpzest-0.1.5/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-29 15:41:00.000000 palimpzest-0.1.5/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-30 00:07:08.000000 palimpzest-0.1.5/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-30 00:07:11.878313 palimpzest-0.1.5/setup.cfg
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.868907 palimpzest-0.1.5/src/
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.870327 palimpzest-0.1.5/src/cli/
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/cli/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/cli/cli_main.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.870786 palimpzest-0.1.5/src/palimpzest/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/__init__.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.871663 palimpzest-0.1.5/src/palimpzest/config/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/config/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/config/config.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/constants.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.871998 palimpzest-0.1.5/src/palimpzest/corelib/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/corelib/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/corelib/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/corelib/schemas.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.872218 palimpzest-0.1.5/src/palimpzest/datamanager/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/datamanager/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11011 2024-05-29 18:18:09.000000 palimpzest-0.1.5/src/palimpzest/datamanager/datamanager.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.872454 palimpzest-0.1.5/src/palimpzest/datasources/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/datasources/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4947 2024-05-29 23:32:36.000000 palimpzest-0.1.5/src/palimpzest/datasources/datasources.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/deploy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.873394 palimpzest-0.1.5/src/palimpzest/elements/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/elements/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/elements/aggregatefunction.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/elements/elements.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/elements/filters.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/elements/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/elements/groupbysig.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/elements/pzlist.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/elements/records.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.873620 palimpzest-0.1.5/src/palimpzest/execution/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      112 2024-05-29 01:56:02.000000 palimpzest-0.1.5/src/palimpzest/execution/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    17615 2024-05-30 00:06:44.000000 palimpzest-0.1.5/src/palimpzest/execution/execution.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.874037 palimpzest-0.1.5/src/palimpzest/generators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/generators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/generators/dspy_utils.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    25348 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/generators/generators.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.874435 palimpzest-0.1.5/src/palimpzest/operators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/operators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/operators/operators.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/operators/physical.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.874939 palimpzest-0.1.5/src/palimpzest/parallel/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/parallel/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/parallel/pzmodal.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.875193 palimpzest-0.1.5/src/palimpzest/policy/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/policy/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/policy/policy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.875691 palimpzest-0.1.5/src/palimpzest/profiler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/profiler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/profiler/attentive_trim.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/profiler/profiler.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/profiler/stats.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.875949 palimpzest-0.1.5/src/palimpzest/sampler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/sampler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/sampler/sampler.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.876177 palimpzest-0.1.5/src/palimpzest/sets/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/sets/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    14861 2024-05-29 18:07:06.000000 palimpzest-0.1.5/src/palimpzest/sets/sets.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.876746 palimpzest-0.1.5/src/palimpzest/solver/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/solver/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/solver/query_strategies.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/solver/solver.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-29 15:41:00.000000 palimpzest-0.1.5/src/palimpzest/solver/task_descriptors.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.877312 palimpzest-0.1.5/src/palimpzest/tools/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/tools/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/tools/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/tools/allenpdf.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/tools/pdfparser.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/tools/skema_tools.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.877665 palimpzest-0.1.5/src/palimpzest/utils/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/utils/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/utils/codegen.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.5/src/palimpzest/utils/sandbox.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:07:11.877838 palimpzest-0.1.5/src/palimpzest.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:07:11.000000 palimpzest-0.1.5/src/palimpzest.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-30 00:07:11.000000 palimpzest-0.1.5/src/palimpzest.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-30 00:07:11.000000 palimpzest-0.1.5/src/palimpzest.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-30 00:07:11.000000 palimpzest-0.1.5/src/palimpzest.egg-info/entry_points.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-30 00:07:11.000000 palimpzest-0.1.5/src/palimpzest.egg-info/requires.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-30 00:07:11.000000 palimpzest-0.1.5/src/palimpzest.egg-info/top_level.txt
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.755237 palimpzest-0.1.6/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-29 15:41:00.000000 palimpzest-0.1.6/LICENSE
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:12:06.755042 palimpzest-0.1.6/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-29 15:41:00.000000 palimpzest-0.1.6/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-30 00:12:03.000000 palimpzest-0.1.6/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-30 00:12:06.755271 palimpzest-0.1.6/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.745690 palimpzest-0.1.6/src/
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.747149 palimpzest-0.1.6/src/cli/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/cli/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/cli/cli_main.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.747607 palimpzest-0.1.6/src/palimpzest/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/__init__.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.748463 palimpzest-0.1.6/src/palimpzest/config/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/config/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/config/config.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/constants.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.748803 palimpzest-0.1.6/src/palimpzest/corelib/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/corelib/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/corelib/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/corelib/schemas.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.749050 palimpzest-0.1.6/src/palimpzest/datamanager/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/datamanager/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11011 2024-05-29 18:18:09.000000 palimpzest-0.1.6/src/palimpzest/datamanager/datamanager.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.749307 palimpzest-0.1.6/src/palimpzest/datasources/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/datasources/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4947 2024-05-29 23:32:36.000000 palimpzest-0.1.6/src/palimpzest/datasources/datasources.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/deploy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.750244 palimpzest-0.1.6/src/palimpzest/elements/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/elements/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/elements/aggregatefunction.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/elements/elements.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/elements/filters.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/elements/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/elements/groupbysig.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/elements/pzlist.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/elements/records.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.750474 palimpzest-0.1.6/src/palimpzest/execution/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      112 2024-05-29 01:56:02.000000 palimpzest-0.1.6/src/palimpzest/execution/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    17549 2024-05-30 00:11:55.000000 palimpzest-0.1.6/src/palimpzest/execution/execution.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.750900 palimpzest-0.1.6/src/palimpzest/generators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/generators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/generators/dspy_utils.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    25348 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/generators/generators.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.751300 palimpzest-0.1.6/src/palimpzest/operators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/operators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/operators/operators.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/operators/physical.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.751600 palimpzest-0.1.6/src/palimpzest/parallel/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/parallel/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/parallel/pzmodal.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.751811 palimpzest-0.1.6/src/palimpzest/policy/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/policy/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/policy/policy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.752326 palimpzest-0.1.6/src/palimpzest/profiler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/profiler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/profiler/attentive_trim.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/profiler/profiler.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/profiler/stats.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.752750 palimpzest-0.1.6/src/palimpzest/sampler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/sampler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/sampler/sampler.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.752973 palimpzest-0.1.6/src/palimpzest/sets/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/sets/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    14861 2024-05-29 18:07:06.000000 palimpzest-0.1.6/src/palimpzest/sets/sets.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.753680 palimpzest-0.1.6/src/palimpzest/solver/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/solver/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/solver/query_strategies.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/solver/solver.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-29 15:41:00.000000 palimpzest-0.1.6/src/palimpzest/solver/task_descriptors.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.754257 palimpzest-0.1.6/src/palimpzest/tools/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/tools/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/tools/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/tools/allenpdf.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/tools/pdfparser.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/tools/skema_tools.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.754648 palimpzest-0.1.6/src/palimpzest/utils/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/utils/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/utils/codegen.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.6/src/palimpzest/utils/sandbox.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-30 00:12:06.754821 palimpzest-0.1.6/src/palimpzest.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-30 00:12:06.000000 palimpzest-0.1.6/src/palimpzest.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-30 00:12:06.000000 palimpzest-0.1.6/src/palimpzest.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-30 00:12:06.000000 palimpzest-0.1.6/src/palimpzest.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-30 00:12:06.000000 palimpzest-0.1.6/src/palimpzest.egg-info/entry_points.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-30 00:12:06.000000 palimpzest-0.1.6/src/palimpzest.egg-info/requires.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-30 00:12:06.000000 palimpzest-0.1.6/src/palimpzest.egg-info/top_level.txt
```

### Comparing `palimpzest-0.1.5/LICENSE` & `palimpzest-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/PKG-INFO` & `palimpzest-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.5
+Version: 0.1.6
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.5/README.md` & `palimpzest-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/pyproject.toml` & `palimpzest-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "palimpzest"
-version = "0.1.5"
+version = "0.1.6"
 description = "Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["relational", "optimization", "llm", "AI programming", "extraction", "tools", "document", "search", "integration"]
 authors = [
     {name="MIT DSG Semantic Management Lab", email="michjc@csail.mit.edu"},
 ]
```

### Comparing `palimpzest-0.1.5/src/cli/cli_main.py` & `palimpzest-0.1.6/src/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/config/config.py` & `palimpzest-0.1.6/src/palimpzest/config/config.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/constants.py` & `palimpzest-0.1.6/src/palimpzest/constants.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/corelib/functions.py` & `palimpzest-0.1.6/src/palimpzest/corelib/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/corelib/schemas.py` & `palimpzest-0.1.6/src/palimpzest/corelib/schemas.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/datamanager/datamanager.py` & `palimpzest-0.1.6/src/palimpzest/datamanager/datamanager.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/datasources/datasources.py` & `palimpzest-0.1.6/src/palimpzest/datasources/datasources.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/elements/aggregatefunction.py` & `palimpzest-0.1.6/src/palimpzest/elements/aggregatefunction.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/elements/elements.py` & `palimpzest-0.1.6/src/palimpzest/elements/elements.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/elements/filters.py` & `palimpzest-0.1.6/src/palimpzest/elements/filters.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/elements/functions.py` & `palimpzest-0.1.6/src/palimpzest/elements/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/elements/groupbysig.py` & `palimpzest-0.1.6/src/palimpzest/elements/groupbysig.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/elements/pzlist.py` & `palimpzest-0.1.6/src/palimpzest/elements/pzlist.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/elements/records.py` & `palimpzest-0.1.6/src/palimpzest/elements/records.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/execution/execution.py` & `palimpzest-0.1.6/src/palimpzest/execution/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,18 @@
         label = "-".join([
             f"{repr(op.model)}_{op.query_strategy if isinstance(op, InduceFromCandidateOp) else None}_{op.token_budget if isinstance(op, InduceFromCandidateOp) else None}"
             for op in ops
         ])
         return f"PZ-{label_idx}-{label}"
 
     @staticmethod
-    def run_sentinel_plan(dataset, plan_idx, num_samples, verbose: bool=False):
+    def run_sentinel_plan(args_tuple):
+        # parse input tuple
+        dataset, plan_idx, num_samples, verbose = args_tuple
+
         # create logical plan from dataset
         logicalTree = dataset.getLogicalTree(num_samples=num_samples, nocache=True)
 
         # compute number of plans
         sentinel_plans = logicalTree.createPhysicalPlanCandidates(sentinels=True)
         plan = sentinel_plans[plan_idx]
 
@@ -310,17 +313,14 @@
         # create logical plan from dataset
         logicalTree = dataset.getLogicalTree(num_samples=num_samples, nocache=True)
 
         # compute number of plans
         sentinel_plans = logicalTree.createPhysicalPlanCandidates(sentinels=True)
         num_sentinel_plans = len(sentinel_plans)
 
-        # short-term hack for colab demo to ensure environment variables are copied into multiprocessing process
-
-
         all_cost_estimate_data, return_records = [], []
         # with Pool(processes=num_sentinel_plans) as pool:
         #     results = pool.starmap(Execute.run_sentinel_plan, [(dataset, plan_idx, num_samples, verbose) for plan_idx in range(num_sentinel_plans)])
         with concurrent.futures.ThreadPoolExecutor(max_workers=num_sentinel_plans) as executor:
             results = list(executor.map(Execute.run_sentinel_plan, [(dataset, plan_idx, num_samples, verbose) for plan_idx in range(num_sentinel_plans)]))
 
             # write out result dict and samples collected for each sentinel
```

### Comparing `palimpzest-0.1.5/src/palimpzest/generators/dspy_utils.py` & `palimpzest-0.1.6/src/palimpzest/generators/dspy_utils.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/generators/generators.py` & `palimpzest-0.1.6/src/palimpzest/generators/generators.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/operators/operators.py` & `palimpzest-0.1.6/src/palimpzest/operators/operators.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/operators/physical.py` & `palimpzest-0.1.6/src/palimpzest/operators/physical.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/parallel/pzmodal.py` & `palimpzest-0.1.6/src/palimpzest/parallel/pzmodal.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/policy/policy.py` & `palimpzest-0.1.6/src/palimpzest/policy/policy.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/profiler/attentive_trim.py` & `palimpzest-0.1.6/src/palimpzest/profiler/attentive_trim.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/profiler/profiler.py` & `palimpzest-0.1.6/src/palimpzest/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/profiler/stats.py` & `palimpzest-0.1.6/src/palimpzest/profiler/stats.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/sets/sets.py` & `palimpzest-0.1.6/src/palimpzest/sets/sets.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/solver/query_strategies.py` & `palimpzest-0.1.6/src/palimpzest/solver/query_strategies.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/solver/solver.py` & `palimpzest-0.1.6/src/palimpzest/solver/solver.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/solver/task_descriptors.py` & `palimpzest-0.1.6/src/palimpzest/solver/task_descriptors.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/tools/allenpdf.py` & `palimpzest-0.1.6/src/palimpzest/tools/allenpdf.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/tools/pdfparser.py` & `palimpzest-0.1.6/src/palimpzest/tools/pdfparser.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/tools/skema_tools.py` & `palimpzest-0.1.6/src/palimpzest/tools/skema_tools.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/utils/codegen.py` & `palimpzest-0.1.6/src/palimpzest/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest/utils/sandbox.py` & `palimpzest-0.1.6/src/palimpzest/utils/sandbox.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest.egg-info/PKG-INFO` & `palimpzest-0.1.6/src/palimpzest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.5
+Version: 0.1.6
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.5/src/palimpzest.egg-info/SOURCES.txt` & `palimpzest-0.1.6/src/palimpzest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.5/src/palimpzest.egg-info/requires.txt` & `palimpzest-0.1.6/src/palimpzest.egg-info/requires.txt`

 * *Files identical despite different names*

