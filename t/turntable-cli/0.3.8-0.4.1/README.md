# Comparing `tmp/turntable_cli-0.3.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/turntable_cli-0.4.1-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,10 @@
-Zip file size: 819412 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-21 16:47 turntable_cli-0.3.8.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-21 16:47 turntable_cli.libs/
--rw-r--r--  2.0 unx     3326 b- defN 23-Nov-21 16:47 turntable.pyi
--rw-r--r--  2.0 unx  2430232 b- defN 23-Nov-21 16:47 turntable.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     4382 b- defN 23-Nov-21 16:47 turntable_cli-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4248 b- defN 23-Nov-21 16:47 turntable_cli-0.3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      697 b- defN 23-Nov-21 16:47 turntable_cli-0.3.8.dist-info/RECORD
--rw-r--r--  2.0 unx       10 b- defN 23-Nov-21 16:47 turntable_cli-0.3.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx      146 b- defN 23-Nov-21 16:47 turntable_cli-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Nov-21 16:47 turntable_cli-0.3.8.dist-info/entry_points.txt
-10 files, 2443094 bytes uncompressed, 817954 bytes compressed:  66.5%
+Zip file size: 759865 bytes, number of entries: 8
+-rw-r--r--  2.0 unx  2208416 b- defN 24-May-30 21:08 turntable.cpython-310-darwin.so
+-rw-r--r--  2.0 unx     3472 b- defN 24-May-30 21:08 turntable.pyi
+-rw-rw-r--  2.0 unx      687 b- defN 24-May-30 21:08 turntable_cli-0.4.1.dist-info/RECORD
+-rw-r--r--  2.0 unx     4382 b- defN 24-May-30 21:08 turntable_cli-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      105 b- defN 24-May-30 21:08 turntable_cli-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-30 21:07 turntable_cli-0.4.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-30 21:07 turntable_cli-0.4.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1045 b- defN 24-May-30 21:08 turntable_cli-0.4.1.dist-info/METADATA
+8 files, 2218170 bytes uncompressed, 758677 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,31 +1,25 @@
-Filename: turntable_cli-0.3.8.dist-info/
-Comment: 
-
-Filename: turntable_cli.libs/
+Filename: turntable.cpython-310-darwin.so
 Comment: 
 
 Filename: turntable.pyi
 Comment: 
 
-Filename: turntable.cpython-311-x86_64-linux-gnu.so
-Comment: 
-
-Filename: turntable_cli-0.3.8.dist-info/LICENSE
+Filename: turntable_cli-0.4.1.dist-info/RECORD
 Comment: 
 
-Filename: turntable_cli-0.3.8.dist-info/METADATA
+Filename: turntable_cli-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: turntable_cli-0.3.8.dist-info/RECORD
+Filename: turntable_cli-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: turntable_cli-0.3.8.dist-info/top_level.txt
+Filename: turntable_cli-0.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: turntable_cli-0.3.8.dist-info/WHEEL
+Filename: turntable_cli-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: turntable_cli-0.3.8.dist-info/entry_points.txt
+Filename: turntable_cli-0.4.1.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## turntable.pyi

```diff
@@ -8,106 +8,112 @@
 # In the future, this will also contain type information for values
 # in the module, so IDEs will use this. Therefore please include it
 # when you make software releases of the extension module that it
 # describes.
 
 import turntable.cli.main
 import turntable.cli.project
+import json
+import pandas
 import turntable.cli.transition
-import github
+import turntable.cli.utils.dataframes
+import turntable.cli.utils.numbers
+import inspect
 import time
 import pydantic
+import github
 import turntable.cli.ci.github_models
-import github.CheckRun
 import turntable.cli.ci.steps.base
-import json
 import logging
 import pathlib
 import enum
-import rich.console
+import turntable.cli.ci.checks.slim_ci
 import copy
-import inspect
 import subprocess
 import turntable.cli.dbt.dialect
 import turntable.cli.dbt.errors
 import turntable.cli.dbt.macros
 import turntable.cli.dbt.templates
 import turntable.cli.preview.validate
 import turntable.cli.utils.strings
 import turntable.cli.utils.files_and_directories
 import re
 import sqlfmt.api
 import sqlfmt.exception
-import itertools
+import logtail
 import sqlglot
-import sqlglot._typing
 import sqlglot.dialects.dialect
 import sqlglot.errors
 import sqlglot.optimizer.isolate_table_selects
 import sqlglot.optimizer.normalize_identifiers
 import sqlglot.optimizer.qualify_columns
 import sqlglot.optimizer.qualify_tables
 import sqlglot.optimizer.scope
 import sqlglot.schema
 import networkx
+import sqlglot._typing
 import sqlglot.expressions
 import sqlglot.optimizer
 import turntable.cli.lib.errors
 import turntable.cli.lineage.parse
 import turntable.cli.utils.graphs
-import string
-import orjson
 import networkx.classes.digraph
 import sqlglot.optimizer.eliminate_ctes
 import sqlglot.optimizer.eliminate_joins
 import sqlglot.optimizer.eliminate_subqueries
 import sqlglot.optimizer.merge_subqueries
 import sqlglot.optimizer.normalize
 import sqlglot.optimizer.optimize_joins
 import sqlglot.optimizer.pushdown_predicates
 import sqlglot.optimizer.pushdown_projections
+import sqlglot.optimizer.qualify
 import sqlglot.optimizer.unnest_subqueries
-import turntable.cli.lineage.custom_qualify
 import typer
+import posthog
 import typing_extensions
-import turntable.cli.ci.checks.dbt_health
 import turntable.cli.ci.github_bot
 import turntable.cli.ci.steps.breaking_changes
 import turntable.cli.ci.steps.cost_optimization
 import turntable.cli.ci.steps.slim_ci
+import turntable.cli.dbt.utils
 import turntable.cli.lib.install
+import turntable.cli.lib.logger
 import turntable.cli.lineage.lineage
 import turntable.cli.modify_yaml
 import turntable.cli.preview.query
-import turntable.cli.ci.checks.slim_ci
 import turntable.cloud.artifacts
+import turntable.cloud.workflows
 import turntable.cli.preview.describe
 import base64
 import ruamel.yaml
 import argparse
 import dataclasses
 import google.cloud
 import ast
 import threading
 import turntable.cli.preview._bq_helper
 import mpire
-import pandas
 import multiprocessing
 import random
-import shutil
+import string
+import turntable.cli.dbt.commands
 import turntable.cli.dbt.profile_helpers
-import turntable.cli.utils.dictionaries
+import turntable.cli.utils.functions
 import turntable.cli.utils.packages
 import dbt.cli.main
 import dbt.adapters.factory
 import dbt.config
 import dbt.events.functions
 import dbt.flags
 import deepmerge
+import shutil
 import contextlib
+import orjson
+import itertools
+import math
 import venv
 import requests
 import turntable.cloud.api
 
 # This is not Python source even if it looks so. Make it clear for
 # now. This was decided by PEP 484 designers.
 __name__ = ...
```

## Comparing `turntable_cli-0.3.8.dist-info/LICENSE` & `turntable_cli-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

