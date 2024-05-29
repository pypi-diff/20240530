# Comparing `tmp/palimpzest-0.1.2.tar.gz` & `tmp/palimpzest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palimpzest-0.1.2.tar", last modified: Wed May 29 18:57:40 2024, max compression
+gzip compressed data, was "palimpzest-0.1.3.tar", last modified: Wed May 29 23:33:11 2024, max compression
```

## Comparing `palimpzest-0.1.2.tar` & `palimpzest-0.1.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.573397 palimpzest-0.1.2/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-29 15:41:00.000000 palimpzest-0.1.2/LICENSE
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-29 18:57:40.573188 palimpzest-0.1.2/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-29 15:41:00.000000 palimpzest-0.1.2/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-29 18:57:05.000000 palimpzest-0.1.2/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-29 18:57:40.573433 palimpzest-0.1.2/setup.cfg
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.563663 palimpzest-0.1.2/src/
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.565146 palimpzest-0.1.2/src/cli/
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/cli/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/cli/cli_main.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.565609 palimpzest-0.1.2/src/palimpzest/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/__init__.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.566520 palimpzest-0.1.2/src/palimpzest/config/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/config/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/config/config.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/constants.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.566851 palimpzest-0.1.2/src/palimpzest/corelib/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/corelib/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/corelib/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/corelib/schemas.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.567080 palimpzest-0.1.2/src/palimpzest/datamanager/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/datamanager/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11011 2024-05-29 18:18:09.000000 palimpzest-0.1.2/src/palimpzest/datamanager/datamanager.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.567351 palimpzest-0.1.2/src/palimpzest/datasources/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/datasources/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4939 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/datasources/datasources.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/deploy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.568317 palimpzest-0.1.2/src/palimpzest/elements/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/elements/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/elements/aggregatefunction.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/elements/elements.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/elements/filters.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/elements/functions.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/elements/groupbysig.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/elements/pzlist.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/elements/records.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.568546 palimpzest-0.1.2/src/palimpzest/execution/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      112 2024-05-29 01:56:02.000000 palimpzest-0.1.2/src/palimpzest/execution/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    16433 2024-05-29 18:56:51.000000 palimpzest-0.1.2/src/palimpzest/execution/execution.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.568970 palimpzest-0.1.2/src/palimpzest/generators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/generators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/generators/dspy_utils.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    25348 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/generators/generators.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.569566 palimpzest-0.1.2/src/palimpzest/operators/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/operators/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/operators/operators.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/operators/physical.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.569838 palimpzest-0.1.2/src/palimpzest/parallel/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/parallel/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/parallel/pzmodal.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.570077 palimpzest-0.1.2/src/palimpzest/policy/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/policy/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/policy/policy.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.570577 palimpzest-0.1.2/src/palimpzest/profiler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/profiler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/profiler/attentive_trim.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/profiler/profiler.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/profiler/stats.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.570823 palimpzest-0.1.2/src/palimpzest/sampler/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/sampler/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/sampler/sampler.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.571041 palimpzest-0.1.2/src/palimpzest/sets/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/sets/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    14861 2024-05-29 18:07:06.000000 palimpzest-0.1.2/src/palimpzest/sets/sets.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.571822 palimpzest-0.1.2/src/palimpzest/solver/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/solver/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/solver/query_strategies.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/solver/solver.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-29 15:41:00.000000 palimpzest-0.1.2/src/palimpzest/solver/task_descriptors.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.572418 palimpzest-0.1.2/src/palimpzest/tools/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/tools/README.md
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/tools/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/tools/allenpdf.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/tools/pdfparser.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/tools/skema_tools.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.572789 palimpzest-0.1.2/src/palimpzest/utils/
--rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/utils/__init__.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/utils/codegen.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.2/src/palimpzest/utils/sandbox.py
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 18:57:40.572953 palimpzest-0.1.2/src/palimpzest.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-29 18:57:40.000000 palimpzest-0.1.2/src/palimpzest.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-29 18:57:40.000000 palimpzest-0.1.2/src/palimpzest.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-29 18:57:40.000000 palimpzest-0.1.2/src/palimpzest.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-29 18:57:40.000000 palimpzest-0.1.2/src/palimpzest.egg-info/entry_points.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-29 18:57:40.000000 palimpzest-0.1.2/src/palimpzest.egg-info/requires.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-29 18:57:40.000000 palimpzest-0.1.2/src/palimpzest.egg-info/top_level.txt
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.431869 palimpzest-0.1.3/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1079 2024-05-29 15:41:00.000000 palimpzest-0.1.3/LICENSE
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-29 23:33:11.431676 palimpzest-0.1.3/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7187 2024-05-29 15:41:00.000000 palimpzest-0.1.3/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2321 2024-05-29 23:32:53.000000 palimpzest-0.1.3/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-05-29 23:33:11.431906 palimpzest-0.1.3/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.422223 palimpzest-0.1.3/src/
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.423731 palimpzest-0.1.3/src/cli/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/cli/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9182 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/cli/cli_main.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.424250 palimpzest-0.1.3/src/palimpzest/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      311 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/__init__.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.425134 palimpzest-0.1.3/src/palimpzest/config/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       27 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/config/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3070 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/config/config.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    12383 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/constants.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.425475 palimpzest-0.1.3/src/palimpzest/corelib/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       48 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/corelib/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3038 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/corelib/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3746 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/corelib/schemas.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.425701 palimpzest-0.1.3/src/palimpzest/datamanager/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       39 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/datamanager/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11011 2024-05-29 18:18:09.000000 palimpzest-0.1.3/src/palimpzest/datamanager/datamanager.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.425960 palimpzest-0.1.3/src/palimpzest/datasources/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/datasources/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4947 2024-05-29 23:32:36.000000 palimpzest-0.1.3/src/palimpzest/datasources/datasources.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/deploy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.426908 palimpzest-0.1.3/src/palimpzest/elements/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      175 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/elements/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      948 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/elements/aggregatefunction.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    10207 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/elements/elements.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1441 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/elements/filters.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      717 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/elements/functions.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2254 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/elements/groupbysig.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1666 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/elements/pzlist.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     3840 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/elements/records.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.427157 palimpzest-0.1.3/src/palimpzest/execution/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      112 2024-05-29 01:56:02.000000 palimpzest-0.1.3/src/palimpzest/execution/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    16433 2024-05-29 18:56:51.000000 palimpzest-0.1.3/src/palimpzest/execution/execution.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.427770 palimpzest-0.1.3/src/palimpzest/generators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       52 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/generators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7141 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/generators/dspy_utils.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    25348 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/generators/generators.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.428166 palimpzest-0.1.3/src/palimpzest/operators/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       49 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/operators/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    43298 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/operators/operators.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    91407 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/operators/physical.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.428460 palimpzest-0.1.3/src/palimpzest/parallel/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/parallel/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1386 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/parallel/pzmodal.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.428676 palimpzest-0.1.3/src/palimpzest/policy/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/policy/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11539 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/policy/policy.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.429174 palimpzest-0.1.3/src/palimpzest/profiler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       75 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/profiler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4720 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/profiler/attentive_trim.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     4677 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/profiler/profiler.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    44230 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/profiler/stats.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.429422 palimpzest-0.1.3/src/palimpzest/sampler/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       22 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/sampler/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      241 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/sampler/sampler.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.429629 palimpzest-0.1.3/src/palimpzest/sets/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       20 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/sets/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    14861 2024-05-29 18:07:06.000000 palimpzest-0.1.3/src/palimpzest/sets/sets.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.430369 palimpzest-0.1.3/src/palimpzest/solver/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       92 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/solver/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    30444 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/solver/query_strategies.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    20606 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/solver/solver.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1465 2024-05-29 15:41:00.000000 palimpzest-0.1.3/src/palimpzest/solver/task_descriptors.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.430941 palimpzest-0.1.3/src/palimpzest/tools/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      483 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/tools/README.md
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/tools/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1813 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/tools/allenpdf.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    11036 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/tools/pdfparser.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     1229 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/tools/skema_tools.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.431296 palimpzest-0.1.3/src/palimpzest/utils/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       45 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/utils/__init__.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9909 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/utils/codegen.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     5778 2024-05-24 18:51:05.000000 palimpzest-0.1.3/src/palimpzest/utils/sandbox.py
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-05-29 23:33:11.431460 palimpzest-0.1.3/src/palimpzest.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9170 2024-05-29 23:33:11.000000 palimpzest-0.1.3/src/palimpzest.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     2143 2024-05-29 23:33:11.000000 palimpzest-0.1.3/src/palimpzest.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-05-29 23:33:11.000000 palimpzest-0.1.3/src/palimpzest.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       41 2024-05-29 23:33:11.000000 palimpzest-0.1.3/src/palimpzest.egg-info/entry_points.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      624 2024-05-29 23:33:11.000000 palimpzest-0.1.3/src/palimpzest.egg-info/requires.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       15 2024-05-29 23:33:11.000000 palimpzest-0.1.3/src/palimpzest.egg-info/top_level.txt
```

### Comparing `palimpzest-0.1.2/LICENSE` & `palimpzest-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/PKG-INFO` & `palimpzest-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.2/README.md` & `palimpzest-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/pyproject.toml` & `palimpzest-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "palimpzest"
-version = "0.1.2"
+version = "0.1.3"
 description = "Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["relational", "optimization", "llm", "AI programming", "extraction", "tools", "document", "search", "integration"]
 authors = [
     {name="MIT DSG Semantic Management Lab", email="michjc@csail.mit.edu"},
 ]
```

### Comparing `palimpzest-0.1.2/src/cli/cli_main.py` & `palimpzest-0.1.3/src/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/config/config.py` & `palimpzest-0.1.3/src/palimpzest/config/config.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/constants.py` & `palimpzest-0.1.3/src/palimpzest/constants.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/corelib/functions.py` & `palimpzest-0.1.3/src/palimpzest/corelib/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/corelib/schemas.py` & `palimpzest-0.1.3/src/palimpzest/corelib/schemas.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/datamanager/datamanager.py` & `palimpzest-0.1.3/src/palimpzest/datamanager/datamanager.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/datasources/datasources.py` & `palimpzest-0.1.3/src/palimpzest/datasources/datasources.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, path: str, dataset_id: str) -> None:
         super().__init__(File, dataset_id)
         self.path = path
         self.idx = 0
 
     def __iter__(self) -> Callable[[], DataRecord]:
         def filteredIterator():
-            for filename in os.listdir(self.path):
+            for filename in sorted(os.listdir(self.path)):
                 file_path = os.path.join(self.path, filename)
                 if os.path.isfile(file_path):
                     dr = DataRecord(self.schema, scan_idx=self.idx)
                     dr.filename = file_path
                     with open(file_path, "rb") as f:
                         dr.contents = f.read()
                     yield dr
```

### Comparing `palimpzest-0.1.2/src/palimpzest/elements/aggregatefunction.py` & `palimpzest-0.1.3/src/palimpzest/elements/aggregatefunction.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/elements/elements.py` & `palimpzest-0.1.3/src/palimpzest/elements/elements.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/elements/filters.py` & `palimpzest-0.1.3/src/palimpzest/elements/filters.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/elements/functions.py` & `palimpzest-0.1.3/src/palimpzest/elements/functions.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/elements/groupbysig.py` & `palimpzest-0.1.3/src/palimpzest/elements/groupbysig.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/elements/pzlist.py` & `palimpzest-0.1.3/src/palimpzest/elements/pzlist.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/elements/records.py` & `palimpzest-0.1.3/src/palimpzest/elements/records.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/execution/execution.py` & `palimpzest-0.1.3/src/palimpzest/execution/execution.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/generators/dspy_utils.py` & `palimpzest-0.1.3/src/palimpzest/generators/dspy_utils.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/generators/generators.py` & `palimpzest-0.1.3/src/palimpzest/generators/generators.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/operators/operators.py` & `palimpzest-0.1.3/src/palimpzest/operators/operators.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/operators/physical.py` & `palimpzest-0.1.3/src/palimpzest/operators/physical.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/parallel/pzmodal.py` & `palimpzest-0.1.3/src/palimpzest/parallel/pzmodal.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/policy/policy.py` & `palimpzest-0.1.3/src/palimpzest/policy/policy.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/profiler/attentive_trim.py` & `palimpzest-0.1.3/src/palimpzest/profiler/attentive_trim.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/profiler/profiler.py` & `palimpzest-0.1.3/src/palimpzest/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/profiler/stats.py` & `palimpzest-0.1.3/src/palimpzest/profiler/stats.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/sets/sets.py` & `palimpzest-0.1.3/src/palimpzest/sets/sets.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/solver/query_strategies.py` & `palimpzest-0.1.3/src/palimpzest/solver/query_strategies.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/solver/solver.py` & `palimpzest-0.1.3/src/palimpzest/solver/solver.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/solver/task_descriptors.py` & `palimpzest-0.1.3/src/palimpzest/solver/task_descriptors.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/tools/allenpdf.py` & `palimpzest-0.1.3/src/palimpzest/tools/allenpdf.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/tools/pdfparser.py` & `palimpzest-0.1.3/src/palimpzest/tools/pdfparser.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/tools/skema_tools.py` & `palimpzest-0.1.3/src/palimpzest/tools/skema_tools.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/utils/codegen.py` & `palimpzest-0.1.3/src/palimpzest/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest/utils/sandbox.py` & `palimpzest-0.1.3/src/palimpzest/utils/sandbox.py`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest.egg-info/PKG-INFO` & `palimpzest-0.1.3/src/palimpzest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palimpzest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Palimpzest is a system which enables anyone to process AI-powered analytical queries simply by defining them in a declarative language
 Author-email: MIT DSG Semantic Management Lab <michjc@csail.mit.edu>
 Project-URL: homepage, https://github.com/mitdbg/palimpzest/
 Project-URL: repository, https://https://github.com/mitdbg/palimpzest/
 Keywords: relational,optimization,llm,AI programming,extraction,tools,document,search,integration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `palimpzest-0.1.2/src/palimpzest.egg-info/SOURCES.txt` & `palimpzest-0.1.3/src/palimpzest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palimpzest-0.1.2/src/palimpzest.egg-info/requires.txt` & `palimpzest-0.1.3/src/palimpzest.egg-info/requires.txt`

 * *Files identical despite different names*

